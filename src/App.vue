<script setup>
import Header from './components/Header.vue'
import CardList from './components/CardList.vue';
import Drawer from './components/Drawer.vue';
</script>

<template>
    <!-- <Drawer /> -->
    <div class="w-4/5 m-auto bg-white rounded-xl shadow-xl mt-14">
        <Header />

        <div class="p-10">
            <div class="flex justify-between items-center mb-8">
                <h2 class="text-3xl font-bold">Все кроссовки</h2>

                <div class="flex gap-4">
                    <select class="py-2 px-3 border rounded-md outline-none bg-white">
                        <option value="">По названию</option>
                        <option value="">По цене (дешевые)</option>
                        <option value="">По цене (дорогие)</option>
                    </select>

                    <div class="relative">
                        <img src="/search.svg" class="absolute left-4 top-3" alt="">
                        <input class="border rounded-md py-2 pl-11 pr-4 outline-none transition focus:border-gray-400"
                            type="text" placeholder="Поиск...">
                    </div>
                </div>
            </div>
            <CardList />

        </div>
    </div>
</template>(15 сентября 2023);

<style scoped></style>