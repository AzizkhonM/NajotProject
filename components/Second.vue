<script setup>
    
    import { advantages } from '../constants/advantages';
        
</script>


<template>
    <div class="m-auto max-w-[1182px]">
        <h1 class="text-[35px] mt-[50px] mb-[50px]">Bizning afzalliklarimiz</h1>
        <div class="grid grid-cols-2">
            <div v-for="el in advantages" class="flex mb-[50px] mr-[60px]">
                <img width="50px" style="height:50px" :src="el.img" alt="">
                <div class="ml-4">
                    <h1 class="text-[22px] mb-[30px] font-bold">{{el.title}}</h1>
                    <h2 class="text-[15px] text-[#607987]">{{ el.text }}</h2>
                </div>
            </div>
        </div>
        <span class="text-[#0EB182] font-bold">Ko‘proq<i class='text-black bx bxs-chevron-down mb-[57px] ml-[20px] p-[10px] rounded-full bg-[#BA8D5B] bg-opacity-10 border-2 border-opacity-5 duration-500 hover:bg-white border-[#BA8D5B] hover:border-opacity-100 cursor-pointer'></i></span>
    </div>
</template>