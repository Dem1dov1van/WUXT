<template>
    <div>
        <Nuxt />
    </div>
</template>

<script>

export default {
  head() {
    return {
      script: [
        {
          src: "https://cdn.tailwindcss.com",
          async: true,
          defer: true
        }
      ]
    }
  }
}
</script>