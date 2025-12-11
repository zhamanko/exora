<script setup>
import { Swiper, SwiperSlide } from 'swiper/vue';
import { Pagination } from 'swiper/modules';
import 'swiper/css/pagination';
import 'swiper/css';
</script>

<template>
    <main class="h-screen snap-y snap-mandatory overflow-y-scroll scroll-smooth">

        <section class="h-screen snap-start flex items-center justify-center text-white bg-cover bg-center bg-no-repeat"
            style="background-image: url('src/img/main-background.jpg');">

            <div class="flex flex-col items-center">
                <div class="flex gap-2 items-center">
                    <img src="/White-logo.png" class="w-12" alt="">
                    <h1 class="text-6xl">EXORA</h1>
                </div>
                <h2 class="text-2xl mt-4">Онлайн-платформа сучасних музеїв</h2>

                <p class=" mt-8 mb-38">Досліджуйте експонати, переглядайте 3D-моделі, занурюйтесь у зали трьох
                    унікальних музеїв — онлайн, у будь-який час.</p>

                <a href="#catalogs"
                    class="bg-white/25 px-8 py-4 rounded-2xl hover:bg-white/40 transition cursor-pointer inline-block">Переглянути
                    музеї</a>
            </div>
        </section>

        <section id="catalogs"
            class="px-4 pt-4 pb-8 h-screen snap-start bg-gradient-to-br from-30% from-black/90 to-gray-500 text-white">
            <div class="flex flex-col items-center h-full">
                <h1 class="text-3xl mb-5 text-center">Наші музеї</h1>

                <div class="w-full flex flex-col gap-4 flex-1">

                    <!-- КАРТКА 1 -->
                    <div class="relative rounded-2xl flex-1 overflow-hidden group">
                        <div style="background-image: url('src/img/museum-1.jpg');"
                            class="absolute inset-0 bg-cover bg-center transition-transform duration-500 group-hover:scale-105">
                        </div>

                        <!-- Градієнт -->
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent transition-opacity duration-500 ">
                        </div>

                        <!-- Контент -->
                        <div class="absolute bottom-0 left-0 right-0 p-6 text-white">
                            <h2 class="text-lg font-semibold">Картка №1</h2>
                            <p class="text-sm opacity-90">Опис музею...</p>
                        </div>
                    </div>

                    <!-- КАРТКА 2 -->
                    <div class="relative rounded-2xl flex-1 overflow-hidden group">
                        <div style="background-image: url('src/img/museum-2.jpg');"
                            class="absolute inset-0 bg-cover bg-center transition-transform duration-500 group-hover:scale-105">
                        </div>

                        <div
                            class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent transition-opacity duration-500 ">
                        </div>

                        <div class="absolute bottom-0 left-0 right-0 p-6 text-white">
                            <h2>Картка №2</h2>
                            <p>Музей мистецтв...</p>
                        </div>
                    </div>

                    <!-- КАРТКА 3 -->
                    <div class="relative rounded-2xl flex-1 overflow-hidden group">
                        <div style="background-image: url('src/img/museum-3.jpg');"
                            class="absolute inset-0 bg-cover bg-center transition-transform duration-500 group-hover:scale-105">
                        </div>

                        <div class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent transiti">
                        </div>

                        <div class="absolute bottom-0 left-0 right-0 p-6 text-white">
                            <h2>Картка №3</h2>
                            <p>Інноваційний музей...</p>
                        </div>
                    </div>

                </div>
            </div>
        </section>

        <selection>

        </selection>


        <section
            class="h-screen p-4 flex flex-col justify-center bg-gradient-to-tr from-30% from-black/90 to-gray-500 items-center snap-start  text-white">
            <h1 class="text-3xl text-center p-5">Музейні події</h1>
            <swiper :slides-per-view="2" :modules="[Pagination]" :pagination="{
                dynamicBullets: true,
            }" :space-between="50" @swiper="onSwiper" @slideChange="onSlideChange" class="h-3/5 w-full">
                <swiper-slide class="rounded-2xl">
                    <img src="https://picsum.photos/600/600" class="w-full h-full rounded-2xl" alt="">
                    <div class=" bg-gray-800/90 absolute bottom-0 left-0 right-0 p-4 rounded-b-2xl">
                        <h2 class="text-lg mb-2">Подія №1</h2>
                        <p class="text-sm opacity-90">Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi
                            praesentium cum tempore beatae, non voluptate totam maxime suscipit doloribus nisi aut animi
                            laboriosam veritatis soluta reprehenderit qui quia iusto fugiat!</p>
                        <span class="text-sm opacity-30 text-end">18.12.2025</span>
                    </div>
                    <div class="absolute top-2 left-2 py-2 px-4 opacity-85 bg-gray-600 rounded-full text-xs">
                        <span>Музей народної архітектури та побуту</span>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <img src="https://picsum.photos/600/600" class="w-full h-full rounded-2xl" alt="">
                    <div class=" bg-gray-800/90 absolute bottom-0 left-0 right-0 p-4 rounded-b-2xl">
                        <h2 class="text-lg mb-2">Подія №1</h2>
                        <p class="text-sm opacity-90">Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi
                            praesentium cum tempore beatae, non voluptate totam maxime suscipit doloribus nisi aut animi
                            laboriosam veritatis soluta reprehenderit qui quia iusto fugiat!</p>
                        <p class="text-sm opacity-30 text-end">18.12.2025</p>
                    </div>
                    <div class="absolute top-2 left-2 py-2 px-4 opacity-85 bg-gray-600 rounded-full text-xs">
                        <span>Музей народної архітектури та побуту</span>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <img src="https://picsum.photos/600/600" class="w-full h-full rounded-2xl" alt="">
                    <div class=" bg-gray-800/90 absolute bottom-0 left-0 right-0 p-4 rounded-b-2xl">
                        <h2 class="text-lg mb-2">Подія №1</h2>
                        <p class="text-sm opacity-90">Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi
                            praesentium cum tempore beatae, non voluptate totam maxime suscipit doloribus nisi aut animi
                            laboriosam veritatis soluta reprehenderit qui quia iusto fugiat!</p>
                        <p class="text-sm opacity-30 text-end">18.12.2025</p>
                    </div>
                    <div class="absolute top-2 left-2 py-2 px-4 opacity-85 bg-gray-600 rounded-full text-xs">
                        <span>Музей №3</span>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <img src="https://picsum.photos/600/600" class="w-full h-full rounded-2xl" alt="">
                    <div class=" bg-gray-800/90 absolute bottom-0 left-0 right-0 p-4 rounded-b-2xl">
                        <h2 class="text-lg mb-2">Подія №1</h2>
                        <p class="text-sm opacity-90">Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi
                            praesentium cum tempore beatae, non voluptate totam maxime suscipit doloribus nisi aut animi
                            laboriosam veritatis soluta reprehenderit qui quia iusto fugiat!</p>
                        <p class="text-sm opacity-30 text-end">18.12.2025</p>
                    </div>
                    <div class="absolute top-2 left-2 py-2 px-4 opacity-85 bg-gray-600 rounded-full text-xs">
                        <span>Музей №3</span>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <img src="https://picsum.photos/600/600" class="w-full h-full rounded-2xl" alt="">
                    <div class=" bg-gray-800/90 absolute bottom-0 left-0 right-0 p-4 rounded-b-2xl">
                        <h2 class="text-lg mb-2">Подія №1</h2>
                        <p class="text-sm opacity-90">Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi
                            praesentium cum tempore beatae, non voluptate totam maxime suscipit doloribus nisi aut animi
                            laboriosam veritatis soluta reprehenderit qui quia iusto fugiat!</p>
                        <p class="text-sm opacity-30 text-end">18.12.2025</p>
                    </div>
                    <div class="absolute top-2 left-2 py-2 px-4 opacity-85 bg-gray-600 rounded-full text-xs">
                        <span>Музей №2</span>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <img src="https://picsum.photos/600/600" class="w-full h-full rounded-2xl" alt="">
                    <div class=" bg-gray-800/90 absolute bottom-0 left-0 right-0 p-4 rounded-b-2xl">
                        <h2 class="text-lg mb-2">Подія №1</h2>
                        <p class="text-sm opacity-90">Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi
                            praesentium cum tempore beatae, non voluptate totam maxime suscipit doloribus nisi aut animi
                            laboriosam veritatis soluta reprehenderit qui quia iusto fugiat!</p>
                        <p class="text-sm opacity-30 text-end">18.12.2025</p>
                    </div>
                    <div class="absolute top-2 left-2 py-2 px-4 opacity-85 bg-gray-600 rounded-full text-xs">
                        <span>Музей №2</span>
                    </div>
                </swiper-slide>
            </swiper>
        </section>

    </main>
</template>

<style>
.swiper {
    padding-bottom: 25px;
}
</style>