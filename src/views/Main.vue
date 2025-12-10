<template>
    <main class="h-screen snap-y snap-mandatory overflow-y-scroll scroll-smooth">

        <section class="h-screen snap-start flex items-center justify-center text-white bg-cover bg-center bg-no-repeat"
            style="background-image: url('/src/img/main-background.jpg');">

            <div class="flex flex-col items-center">
                <h1 class="text-5xl">Exora</h1>
                <h2 class="text-2xl mt-4">Онлайн-платформа сучасних музеїв</h2>

                <p class=" mt-8 mb-38">Досліджуйте експонати, переглядайте 3D-моделі, занурюйтесь у зали трьох
                    унікальних музеїв — онлайн, у будь-який час.</p>

                <a href="#catalogs"
                    class="bg-white/25 px-8 py-4 rounded-2xl hover:bg-white/40 transition cursor-pointer inline-block">Переглянути
                    музеї</a>
            </div>
        </section>

        <section id="catalogs" class="px-4 pt-4 pb-8 h-screen snap-start bg-black/90 text-white">
            <div class="flex flex-col items-center h-full">
                <h1 class="text-2xl mb-5 text-center">Наші музеї</h1>

                <div class="w-full flex flex-col gap-4 flex-1">

                    <!-- КАРТКА 1 -->
                    <div class="relative rounded-2xl flex-1 overflow-hidden group">
                        <div style="background-image: url('/src/img/museum-1.jpg');"
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
                        <div style="background-image: url('/src/img/museum-2.jpg');"
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
                        <div style="background-image: url('/src/img/museum-3.jpg');"
                            class="absolute inset-0 bg-cover bg-center transition-transform duration-500 group-hover:scale-105">
                        </div>

                        <div
                        class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent transiti">
                        </div>

                        <div class="absolute bottom-0 left-0 right-0 p-6 text-white">
                            <h2>Картка №3</h2>
                            <p>Інноваційний музей...</p>
                        </div>
                    </div>

                </div>
            </div>
        </section>



        <section class="h-screen snap-start flex items-center justify-center bg-green-400 text-white">
            <h1 class="text-5xl">3</h1>
        </section>

    </main>
</template>
