<script>
export default {
    data() {
        return {
            src: null
        }
    },
    props: {
        imageId: Number
    },
    async mounted() {
        const response = await fetch(`${this.$wp._options.endpoint}wp/v2/media/${this.imageId}`)
        let json
        if (response.ok) {
            json = await response.json()
        }
        this.src = json.source_url
    }
}
</script>

<template>
    <img :src="src ? src : './image-not-found.png'" />
</template>