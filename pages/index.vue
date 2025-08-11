<script setup lang="ts">
</script>

<template>
    <div class="max-w-full min-h-screen">
        <div class="text-center py-8 sm:py-10">
            <h1 class="text-2xl sm:text-3xl md:text-4xl font-bold">โครงงานของฉัน</h1>
        </div>

        <div class="px-4 sm:px-6 md:px-10 flex justify-center">
            <!-- กล่องหลัก (responsive) -->
            <div class="w-full max-w-5xl lg:max-w-6xl rounded-3xl border-2 border-blue-600 p-4 sm:p-8 md:p-12">
                <ul class="space-y-4 sm:space-y-6">
                    <!-- แถวที่ 1 -->
                    <li
                        class="flex flex-col sm:grid sm:grid-cols-[auto_1fr_auto_auto] items-center gap-3 sm:gap-6 py-4 sm:py-6 border-b last:border-b-0">
                        <div class="flex items-center gap-4 sm:gap-6">
                            <span
                                class="h-12 w-12 sm:h-14 sm:w-14 md:h-16 md:w-16 rounded-full border border-gray-400 flex items-center justify-center text-lg sm:text-xl md:text-2xl">1</span>
                            <span class="text-base sm:text-lg md:text-xl">ยื่นขอสอบหัวข้อ</span>
                        </div>
                        <span
                            class="text-base sm:text-lg md:text-xl text-gray-700 sm:justify-self-center mt-1 sm:mt-0">ยังไม่ยื่นสอบ</span>
                        <button
                            class="mt-2 sm:mt-0 h-10 w-10 sm:h-12 sm:w-12 md:h-14 md:w-14 rounded-full border border-gray-400 flex items-center justify-center text-2xl md:text-3xl leading-none">+</button>
                    </li>

                    <!-- แถวที่ 2 -->
                    <li
                        class="flex flex-col sm:grid sm:grid-cols-[auto_1fr_auto_auto] items-center gap-3 sm:gap-6 py-4 sm:py-6 border-b last:border-b-0">
                        <div class="flex items-center gap-4 sm:gap-6">
                            <span
                                class="h-12 w-12 sm:h-14 sm:w-14 md:h-16 md:w-16 rounded-full border border-gray-400 flex items-center justify-center text-lg sm:text-xl md:text-2xl">2</span>
                            <span class="text-base sm:text-lg md:text-xl">ทำโปรแกรม</span>
                        </div>
                        <span
                            class="text-base sm:text-lg md:text-xl text-gray-700 sm:justify-self-center mt-1 sm:mt-0">0%</span>
                        <button
                            class="mt-2 sm:mt-0 h-10 w-10 sm:h-12 sm:w-12 md:h-14 md:w-14 rounded-full border border-gray-400 flex items-center justify-center text-2xl md:text-3xl leading-none">+</button>
                    </li>

                    <!-- แถวที่ 3 -->
                    <li
                        class="flex flex-col sm:grid sm:grid-cols-[auto_1fr_auto_auto] items-center gap-3 sm:gap-6 py-4 sm:py-6 border-b last:border-b-0">
                        <div class="flex items-center gap-4 sm:gap-6">
                            <span
                                class="h-12 w-12 sm:h-14 sm:w-14 md:h-16 md:w-16 rounded-full border border-gray-400 flex items-center justify-center text-lg sm:text-xl md:text-2xl">3</span>
                            <span class="text-base sm:text-lg md:text-xl">เล่มบัณฑิตนิพนธ์</span>
                        </div>
                        <span
                            class="text-base sm:text-lg md:text-xl text-gray-700 sm:justify-self-center mt-1 sm:mt-0">0%</span>
                        <button
                            class="mt-2 sm:mt-0 h-10 w-10 sm:h-12 sm:w-12 md:h-14 md:w-14 rounded-full border border-gray-400 flex items-center justify-center text-2xl md:text-3xl leading-none">+</button>
                    </li>

                    <!-- แถวที่ 4 -->
                    <li
                        class="flex flex-col sm:grid sm:grid-cols-[auto_1fr_auto_auto] items-center gap-3 sm:gap-6 py-4 sm:py-6 border-b last:border-b-0">
                        <div class="flex items-center gap-4 sm:gap-6">
                            <span
                                class="h-12 w-12 sm:h-14 sm:w-14 md:h-16 md:w-16 rounded-full border border-gray-400 flex items-center justify-center text-lg sm:text-xl md:text-2xl">4</span>
                            <span class="text-base sm:text-lg md:text-xl">ยื่นขอสอบจบ</span>
                        </div>
                        <span
                            class="text-base sm:text-lg md:text-xl text-gray-700 sm:justify-self-center mt-1 sm:mt-0">ยังไม่ยื่นสอบจบ</span>
                        <button
                            class="mt-2 sm:mt-0 h-10 w-10 sm:h-12 sm:w-12 md:h-14 md:w-14 rounded-full border border-gray-400 flex items-center justify-center text-2xl md:text-3xl leading-none">+</button>
                    </li>

                    <!-- แถวที่ 5 -->
                    <li
                        class="flex flex-col sm:grid sm:grid-cols-[auto_1fr_auto_auto] items-center gap-3 sm:gap-6 py-4 sm:py-6">
                        <div class="flex items-center gap-4 sm:gap-6">
                            <span
                                class="h-12 w-12 sm:h-14 sm:w-14 md:h-16 md:w-16 rounded-full border border-gray-400 flex items-center justify-center text-lg sm:text-xl md:text-2xl">5</span>
                            <span class="text-base sm:text-lg md:text-xl">ส่งเล่มและโปรแกรม</span>
                        </div>
                        <span
                            class="text-base sm:text-lg md:text-xl text-gray-700 sm:justify-self-center mt-1 sm:mt-0">&nbsp;</span>
                        <button
                            class="mt-2 sm:mt-0 h-10 w-10 sm:h-12 sm:w-12 md:h-14 md:w-14 rounded-full border border-gray-400 flex items-center justify-center text-2xl md:text-3xl leading-none">+</button>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style scoped></style>
