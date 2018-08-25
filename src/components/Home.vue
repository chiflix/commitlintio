<template>
  <b-container fluid>
    <b-row class="navbar">
      <b-col class="title">
        CIMMIT<span class="lighter">LINT</span>
      </b-col>
      <b-col class="slogan text-left d-none d-md-block" cols="4">
        lint commit messages online
      </b-col>
      <b-col class="rules">
        rules: Angular
      </b-col>
    </b-row>
    <b-row class="mainContainer">
      <b-col>
        <Linter></Linter>
      </b-col>
    </b-row>
    <b-row>
        <b-col class="text-left">
          <Footer></Footer>
        </b-col>
    </b-row>
    <b-row class="ads">
      <b-col>
        <script2>
         (adsbygoogle = window.adsbygoogle || []).push({
              google_ad_client: "ca-pub-3236699304584559",
              enable_page_level_ads: true
         });
        </script2>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import Linter from './Linter';
import Footer from './Footer';

export default {
  name: 'Home',
  components: {
    Linter,
    Footer,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.navbar {
  min-height: 4.1667em;
  height: 5.4167em;
}
.title {
  color: #f1f8fd;
  font-size: 2em;
  font-family: 'Oswald', sans-serif;
}
.title .lighter {
  color: #b2dde5;
}
.mainContainer {
  background-color: #453E48;
  padding: 3.5em 0;
}
</style>
