<script setup>

    import { courses } from '../constants/courses';

</script>


<template>
    <div class="py-[52px] bg-[#F9F8F7]">
        <div class="m-auto max-w-[1182px] pt-[22px] pb-[8px] pl-[35px]">
            <h1 class="font-extrabold text-[35px] mb-[26px]">Yo‘nalishlar bo‘yicha kurslar</h1>
            <h2 class="text-[#607987] text-[19px] font-semibold">Zamonaviy sohalardan birini o‘rganing va talabgir kasb egasi bo‘ling!</h2>
            <div class="grid grid-cols-4 gap-x-[35px] mb-[20px]">
                <div v-for="el in courses" class="rounded-md border border-black pl-[20px] mt-[27px] hover:bg-white hover:border-white duration-500 hover:shadow-md">
                    <h1 class="mt-[18px] mb-15px">{{ el.title }}</h1>
                    <h2 class="mb-[18px] text-[#607987]">{{ el.text }}</h2>
                </div>
            </div>
            <h1 class="text-[#0EB182] text-[18px] font-bold">Barcha kurslarni ko‘rish</h1>
        </div>
    </div>
</template>