<template>
  <div class="home">
    <section class="hero">
      <div class="container">
        <div class="title">Soaring to new heights</div>
        <div class="row">
          <div class="col l10">
            {{ subheading }}
          </div>
        </div>
        <a class="waves-effect waves-light btn">OUR SERVICES</a>
      </div>
    </section>
    <section>
      <div class="container pt-2">
        <div class="row">
          <div class="col m2">
            <a>
              <font-awesome-icon
                :icon="['fas', 'cog']"
                size="3x"
                class="teal-text text-lighten-2"
              />
            </a>
          </div>
          <div class="col m5">
            <b>
              We provide a superior logistic so that your business can succeed
              in a crazy world
            </b>
          </div>
          <div class="col m5">
            Et esse audire complectitur duo, epicuri eleifend mandamus in vis.
            Ne corrumpit maiestatis reprimique ius, cum eu quis aliquid
            appareat.
          </div>
        </div>
      </div>
    </section>
    <div class="container">
      <div class="row">
        <div class="col s12 m6 l4">
          <div class="card small">
            <div class="card-content">
              Eam ut ubique deserunt definitiones, duo ferri tollit iisque ne,
              id scripta omittantur usu. Mea ei reque discere, omnis viderer quo
              te. In vocibus tacimates per.
            </div>
            <div class="card-title right-align grey-text lighten-2">
              <i class="p-2">- John Doe</i>
            </div>
          </div>
        </div>
        <div class="col s12 m6 l4">
          <div class="card small">
            <div class="card-content">
              Clita tempor nostro his ad, sit vocent evertitur no. Ex eos sale
              erant recusabo, ea sea enim scaevola. Eu unum persecuti
              concludaturque vis, veri electram urbanitas ne mei.
            </div>
            <div class="card-title right-align grey-text lighten-2">
              <i class="p-2">- Francis Lux</i>
            </div>
          </div>
        </div>
        <div class="col s12 m6 l4">
          <div class="card small">
            <div class="card-content">
              Eam in tibique democritum, paulo mundi impedit pri ea, omnes
              labores appellantur cu his. Libris eleifend nam ea, nisl case et
              mea.
            </div>
            <div class="card-title right-align grey-text lighten-2">
              <i class="p-2">- Kevin Blocq</i>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "home",
  data() {
    return {
      heading: "Soaring to new heights",
      subheading:
        "Ex cum habeo semper scriptorem, erant disputando at pri. Ea libris mentitum delicata qui. Te velit iriure denique duo. Mei at clita ceteros. Ex duo fugit delenit accusamus, eu semper virtute suscipit nec, his ut adhuc animal."
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
