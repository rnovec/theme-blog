<template>
  <v-container
    id="about"
    tag="section"
  >
    <vue-markdown>
      {{about_text}}
    </vue-markdown>
  </v-container>
</template>

<script>
  import VueMarkdown from 'vue-markdown';
  import about_text from '../../../public/static/about.md';

  export default {
    name: 'About',
    data: () => {
      return {
        about_text: about_text
      }
    },
    components: {
      VueMarkdown
    }
  }
</script>
