<template>
  <Nuxt />
</template>
<script>
  export default {
    data() {
      return {
        title: 'My Slides'
      }
    },
    head() {
      return {
        title: this.title,
        script: [
          // hid is used as unique identifier. Do not use `vmid` for it as it will not work
          {
            hid: 'revealjs',
            src: 'src="https://cdnjs.cloudflare.com/ajax/libs/reveal.js/4.2.1/reveal.js"'
          }
        ],
        link: [
          {
            hid: 'revealcss',
            rel: 'stylesheet',
            href: 'https://cdnjs.cloudflare.com/ajax/libs/reveal.js/4.2.1/reveal.min.css'
          },
          {
            hid: 'revealtheme',
            rel: 'stylesheet',
            href: 'https://cdnjs.cloudflare.com/ajax/libs/reveal.js/4.2.1/theme/sky.min.css'
          }
        ]
      }
    }
  }
</script>
