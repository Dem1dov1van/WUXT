<template>
  <div>
    <nuxt class="container"/>
  </div>
</template>

<script>
import Logo from '~/components/Logo'

export default {
  components: {
    Logo
  },
  head() {
    return {
      script: [
        {
          src: "https://cdn.tailwindcss.com",
          async: true,
          defer: true
        },
        {
          src: "https://cdn.jsdelivr.net/npm/@fancyapps/ui@5.0/dist/fancybox/fancybox.umd.js"
        }
      ],
      link: [
        {
          href: "https://cdn.jsdelivr.net/npm/@fancyapps/ui@5.0/dist/fancybox/fancybox.css",
          rel: "stylesheet"
        }
      ]
    }
  },
  mounted() {
    Fancybox.bind('[data-fancybox]', {
        // Your custom options
      }); 
  }
}
</script>


<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Nunito:700,600,400|Open+Sans:400,700');
$primary: #37495c;
$secondary: #48b884;

html,
body {
  margin: 0;
  padding: 0;
}

html {
  font-family: 'Open Sans', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

a {
  color: #48b884;
  text-decoration: none;

  &:hover {
    color: darken($color: #48b884, $amount: 10);
  }
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: 'Nunito';
  font-weight: 700;
}

.container {
  width: 100%;
  margin: 0 auto;
  padding-right: 15px;
  padding-left: 15px;
}
</style>
