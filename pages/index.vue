<script setup lang="ts">
const tasks = [
    { title: "ยื่นขอสอบหัวข้อ", status: "ยังไม่ยื่นสอบ" },
    { title: "ทำโปรแกรม", status: "0%" },
    { title: "เล่มบัณฑิตนิพนธ์", status: "0%" },
    { title: "ยื่นขอสอบจบ", status: "ยังไม่ยื่นสอบจบ" },
    { title: "ส่งเล่มและโปรแกรม", status: "" },
];
</script>

<template>
    <div class="max-w-full min-h-screen bg-gray-50">
        <!-- หัวข้อ -->
        <div class="text-center py-8 sm:py-10">
            <h1 class="text-2xl sm:text-3xl md:text-4xl font-bold text-gray-800">
                โครงงานของฉัน
            </h1>
        </div>

        <div class="px-4 sm:px-6 md:px-10 flex justify-center">
            <!-- กล่องหลัก -->
            <div
                class="w-full max-w-5xl lg:max-w-6xl rounded-3xl border-2 border-blue-600 p-4 sm:p-8 md:p-12 bg-white shadow-lg">
                <ul class="divide-y divide-gray-200">
                    <li v-for="(item, index) in tasks" :key="index"
                        class="flex items-center justify-between gap-3 py-4 sm:py-6 hover:bg-blue-50 transition flex-wrap">
                        <!-- หมายเลข + ชื่อ -->
                        <div class="flex items-center gap-4 min-w-[150px]">
                            <span
                                class="h-12 w-12 sm:h-14 sm:w-14 md:h-16 md:w-16 rounded-full border border-gray-400 flex items-center justify-center text-lg sm:text-xl md:text-2xl font-semibold text-gray-700 bg-white">
                                {{ index + 1 }}
                            </span>
                            <span class="text-base sm:text-lg md:text-xl font-medium text-gray-800">
                                {{ item.title }}
                            </span>
                        </div>

                        <!-- สถานะ -->
                        <span class="text-base sm:text-lg md:text-xl text-gray-600 text-center flex-1">
                            {{ item.status || "—" }}
                        </span>

                        <!-- ปุ่ม -->
                        <button
                            class="h-10 w-10 sm:h-12 sm:w-12 md:h-14 md:w-14 rounded-full border border-gray-400 flex items-center justify-center text-2xl md:text-3xl leading-none text-gray-600 hover:bg-blue-600 hover:text-white hover:border-blue-600 transition">
                            +
                        </button>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style scoped></style>
