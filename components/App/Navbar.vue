<script setup lang="ts">
import { ref } from 'vue'

const isOpen = ref(false)
</script>

<template>
    <header class="sticky top-0 z-50 shadow-sm">
        <nav class="bg-white border-b border-gray-200">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-10">
                <div class="flex justify-between items-center h-16">
                    <!-- เมนูซ้าย -->
                    <div class="flex items-center">
                        <!-- ปุ่มมือถือ -->
                        <button @click="isOpen = !isOpen"
                            class="md:hidden p-2 rounded-md hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-blue-500">
                            <svg class="h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                                stroke="currentColor">
                                <path v-if="!isOpen" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                    d="M4 6h16M4 12h16M4 18h16" />
                                <path v-else stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                    d="M6 18L18 6M6 6l12 12" />
                            </svg>
                        </button>

                        <!-- เมนู Desktop -->
                        <ul class="hidden md:flex space-x-6 font-semibold text-gray-700">
                            <li>
                                <NuxtLink to="/graduate-thesis" class="hover:text-blue-600 transition">ค้นหาโครงงาน
                                </NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/" class="hover:text-blue-600 transition">ขั้นตอนการทำโครงงาน</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/" class="hover:text-blue-600 transition">คู่มือการทำบัณฑิตนิพนธ์
                                </NuxtLink>
                            </li>
                        </ul>
                    </div>

                    <!-- ขวา: ชื่อผู้ใช้ -->
                    <div>
                        <NuxtLink to="/login"
                            class="border border-gray-300 hover:bg-blue-600 hover:text-white text-gray-700 transition rounded-md px-4 py-2 cursor-pointer text-sm sm:text-base">
                            ณัฐภัทร ภูมิเมฆ
                        </NuxtLink>
                    </div>
                </div>
            </div>

            <!-- เมนูมือถือ -->
            <div v-show="isOpen" class="md:hidden border-t border-gray-200">
                <ul class="flex flex-col space-y-2 p-4 font-semibold text-gray-700">
                    <li>
                        <NuxtLink to="/graduate-thesis" class="block hover:text-blue-600 transition"
                            @click="isOpen = false">ค้นหาโครงงาน</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/" class="block hover:text-blue-600 transition" @click="isOpen = false">
                            ขั้นตอนการทำโครงงาน</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/" class="block hover:text-blue-600 transition" @click="isOpen = false">
                            คู่มือการทำบัณฑิตนิพนธ์</NuxtLink>
                    </li>
                </ul>
            </div>
        </nav>
    </header>
</template>

<style scoped></style>
