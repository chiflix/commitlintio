<template>
  <b-container class="footer" v-html="compiledMarkdown">
  </b-container>
</template>

<script>
import marked from 'marked';
import msg from '../helper/messages';

export default {
  name: 'Footer',
  computed: {
    compiledMarkdown() {
      return marked(msg, { sanitize: true });
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.footer {
  color: #fefeff;
  padding: 0.8em;
  max-width: 40em;
}
</style>
