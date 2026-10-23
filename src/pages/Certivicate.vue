<script setup>
import Footer from '../components/Footer.vue';
import HeaderAbout from '../components/HeaderAbout.vue';

</script>

<template>
    <div>
        <HeaderAbout image="/assets/about/hero_profile_perusahaan.jpg" title="Perusahaan" breadcrumb="Sertifikat"/>

        <div class="px-6 md:px-16 lg:px-24 xl:px-32 py-20">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-5">
                <div v-for="value in 6" class="flex flex-col bg-white shadow-xl border border-gray-300 rounded overflow-hidden hover:shadow-2xl hover:scale-[1.02] transition-all duration-300">
                    <div class="w-full h-48 sm:h-56 md:h-60">
                        <img src="https://i.pinimg.com/1200x/d6/68/08/d66808a0baab3cff54bdccfd952c8ec9.jpg" class="w-full h-full object-cover" />
                    </div>

                    <div class="flex flex-col justify-between h-full pt-5 pb-10 px-5">
                        <h1 class="text-lg sm:text-xl md:text-xl font-semibold mb-5 text-slate-800">
                            Sertifikat BPJS Kesehatan
                        </h1>
                        <p class="text-gray-600">BPJS</p>
                    </div>
                </div>
            </div>
        </div>

        <Footer/>
    </div>

</template>