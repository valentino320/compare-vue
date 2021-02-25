<template>
  <div class="faq">
    <section class="">
      <div class="container">
        <div class="title">FAQ</div>
        <div class="row">
          <div class="col l10">
            {{ subheading }}
          </div>
        </div>
      </div>
    </section>

    <div class="container">
      <div class="row" v-if="faqs && faqs.length">
        <div class="col s12 m6 l4" v-for="faq of faqs">
          <div class="card medium">
            <div class="card-content">
              <span class="card-title">
                {{ faq.title }}
              </span>
              <p>{{ faq.body }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  name: "Faq",
  data: () => ({
    faqs: [],
    errors: [],
    subheading:
      "Pro ex fugit ullum voluptaria, accusam luptatum vis ut. Ad sonet concludaturque cum. Mel eu essent temporibus. Ei ius ceteros convenire disputando. Unum causae neglegentur nec ex, qui ad tota audire."
  }),
  created() {
    axios
      .get("http://jsonplaceholder.typicode.com/posts")
      .then(response => {
        this.faqs = response.data.slice(0, 10);
      })
      .catch(e => {
        this.errors.push(e);
      });
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
