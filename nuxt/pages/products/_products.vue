<template>
    <div v-if="data">
        <div class="grid grid-cols-1 gap-4 lg:grid-cols-3 lg:gap-8 mt-6">
            <div class="grid gap-4 lg:col-span-2">
                <div>
                    <a 
                        :href="data.img" 
                        data-fancybox="gallery" 
                        data-caption="Caption #1"
                    >
                        <img 
                            class="h-auto max-w-full rounded-lg" 
                            :src="data.img" 
                            alt=""  
                        >
                    </a>
                </div>
                <div class="grid grid-cols-5 gap-4">
                    <div 
                        v-for="(photo, i) in data.photos"
                        :key="i"
                    >
                        <a 
                            :href="photo.url" 
                            data-fancybox="gallery" 
                            data-caption="Caption #1"
                        >
                            <img 
                                class="h-auto max-w-full rounded-lg"   
                                :src="photo.url" 
                                alt=""
                            >
                        </a>
                    </div>
                    <div>
                        <a href="https://flowbite.s3.amazonaws.com/docs/gallery/square/image-2.jpg" data-fancybox="gallery" data-caption="Caption #2">
                            <img class="h-auto max-w-full rounded-lg" src="https://flowbite.s3.amazonaws.com/docs/gallery/square/image-2.jpg" alt="">
                        </a>
                    </div>
                    <div>
                        <a href="https://flowbite.s3.amazonaws.com/docs/gallery/square/image-3.jpg" data-fancybox="gallery" data-caption="Caption #3">
                            <img class="h-auto max-w-full rounded-lg" src="https://flowbite.s3.amazonaws.com/docs/gallery/square/image-3.jpg" alt="">
                        </a>
                    </div>
                    <div>
                        <a href="https://flowbite.s3.amazonaws.com/docs/gallery/square/image-4.jpg" data-fancybox="gallery" data-caption="Caption #4">
                            <img class="h-auto max-w-full rounded-lg" src="https://flowbite.s3.amazonaws.com/docs/gallery/square/image-4.jpg" alt="">
                        </a>
                    </div>
                    <div>
                        <a href="https://flowbite.s3.amazonaws.com/docs/gallery/square/image-5.jpg" data-fancybox="gallery" data-caption="Caption #5">
                            <img class="h-auto max-w-full rounded-lg" src="https://flowbite.s3.amazonaws.com/docs/gallery/square/image-5.jpg" alt="">
                        </a>
                    </div>
                    <div>
                        <a href="https://flowbite.s3.amazonaws.com/docs/gallery/square/image-6.jpg" data-fancybox="gallery" data-caption="Caption #6">
                            <img class="h-auto max-w-full rounded-lg" src="https://flowbite.s3.amazonaws.com/docs/gallery/square/image-6.jpg" alt="">
                        </a>
                    </div>
                </div>
            </div>

            <div class="flow-root rounded-lg border border-gray-100 py-3 shadow-sm">
                <dl class="-my-3 divide-y divide-gray-100 text-sm">
                    <div class="grid grid-cols-1 gap-1 p-3 sm:grid-cols-3 sm:gap-4">
                    <dt class="font-medium text-gray-900">productId</dt>
                    <dd class="text-gray-700 sm:col-span-2" v-html="productId"></dd>
                    </div>

                    <div class="grid grid-cols-1 gap-1 p-3 sm:grid-cols-3 sm:gap-4">
                    <dt class="font-medium text-gray-900">Что это?</dt>
                    <dd class="text-gray-700 sm:col-span-2">Стул барный</dd>
                    </div>

                    <div class="grid grid-cols-1 gap-1 p-3 sm:grid-cols-3 sm:gap-4">
                    <dt class="font-medium text-gray-900">Где находится</dt>
                    <dd class="text-gray-700 sm:col-span-2">Бар на цвт19</dd>
                    </div>

                    <div class="grid grid-cols-1 gap-1 p-3 sm:grid-cols-3 sm:gap-4">
                    <dt class="font-medium text-gray-900">Цена</dt>
                    <dd class="text-gray-700 sm:col-span-2">1 999 Р</dd>
                    </div>

                    <div class="grid grid-cols-1 gap-1 p-3 sm:grid-cols-3 sm:gap-4">
                    <dt class="font-medium text-gray-900">Описание</dt>
                    <dd class="text-gray-700 sm:col-span-2">
                        Преобразите ваше пространство с нашим стильным барным стулом. Этот барный стул сочетает в себе современный дизайн и непревзойденный комфорт, делая его идеальным дополнением для кухонного островка, бара или обеденной зоны.
                    </dd>
                    </div>
                </dl>
            </div>
        </div>

        <span class="flex items-center my-10">
            <span class="h-px flex-1 bg-black"></span>
            <span class="shrink-0 px-6">S Store</span>
            <span class="h-px flex-1 bg-black"></span>
        </span>

        <section>
            <div class="w-full bg-white rounded-lg border p-2">

            <h3 class="font-bold">Участники:</h3>

            <form>

                <div class="flex flex-col">

                    <div class="border rounded-md p-3 ml-3 my-3">
                        <div class="flex gap-3 items-center">

                            <img src="https://avatars.githubusercontent.com/u/22263436?v=4"
                                class="object-cover w-8 h-8 rounded-full 
                                border-2 border-emerald-400  shadow-emerald-400
                                ">

                            <h3 class="font-bold">
                                Елена Епишина
                            </h3>
                        </div>


                        <p class="text-gray-600 mt-2">
                            Хочу красный кожаный стул!
                        </p>

                    </div>

                    <div class="border rounded-md p-3 ml-3 my-3">
                        <div class="flex gap-3 items-center">

                            <img src="https://avatars.githubusercontent.com/u/22263436?v=4"
                                class="object-cover w-8 h-8 rounded-full 
                                border-2 border-emerald-400  shadow-emerald-400
                                ">

                            <h3 class="font-bold">
                                Олег Игоревич
                            </h3>
                        </div>


                        <p class="text-gray-600 mt-2">
                            Тоже не против забрать себе такой)
                        </p>
                    </div>
                </div>



                <div class="w-full px-3 my-2">
                    <textarea
                        class="bg-gray-100 rounded border border-gray-400 leading-normal resize-none w-full h-20 py-2 px-3 font-medium placeholder-gray-700 focus:outline-none focus:bg-white"
                        name="body" placeholder='Оставь комментарий, если хочешь себе этот предмет' required></textarea>
                </div>

                <div class="w-full flex justify-end px-3">
                    <input type='submit' class="px-2.5 py-1.5 rounded-md text-white text-sm bg-indigo-500" value='Отправить'>
                </div>
            </form>

            </div>
        </section>

    </div>

</template>

<script>
import EnvelopeImage from '../../components/EnvelopeImage.vue'
export default {
  components: { EnvelopeImage },
    data() {
        return {
            productId: null,
            data: null
        }
    },
    async mounted() {
        this.productId = this.$route.params.products
        const response = await fetch(`${this.$wp._options.endpoint}wp/v2/products/${this.productId}?acf_format=standard`)
        let json
        if (response.ok) {
            json = await response.json()
        }
        this.data = json.acf
        console.log(this.data, 'this.data')
    },
    methods: {
        getProductById () {
            this.productId = this.$route.params.products
        },
        async getHrefById (id) {
            const response = await fetch(`${this.$wp._options.endpoint}wp/v2/media/${id}`)
            let json
            if (response.ok) {
                json = await response.json()
            }
            return json.source_url || ''
        }
    }
}
</script>