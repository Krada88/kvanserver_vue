<template>
  <div class="wrapper">
    <header_div/>
      <nuxt/>
    <footer_div/>
  </div>
</template>

<script>

  import Header_div from '~/components/Header.vue'
  import Footer_div from '~/components/Footer.vue'


  export default {
    components: {
      Header_div,
      Footer_div
    }
  }
</script>
