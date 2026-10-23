<script setup>
import Footer from '../components/Footer.vue';
import HeaderAbout from '../components/HeaderAbout.vue';
import { listPartners } from '../data/services.js';

</script>

<template>
    <div>
        <HeaderAbout image="/assets/about/hero_profile_perusahaan.jpg" title="Perusahaan" breadcrumb="Partner"/>

        <div class="py-20 px-6 md:px-16 lg:px-24 xl:px-32">
            <div class="flex flex-col">
                <h1 class="text-2xl md:text-4xl font-semibold mb-4 text-slate-800">Partners</h1>
                <div class="grid grid-cols-2 md:grid-cols-2 lg:grid-cols-4 gap-5">
                    <div v-for="item in listPartners" :key="item.id" class="w-full">
                        <img :src="item.img" alt="" class="h-44 object-contain w-full">
                    </div>
                </div>
            </div>
        </div>

        <Footer/>
    </div>

</template>