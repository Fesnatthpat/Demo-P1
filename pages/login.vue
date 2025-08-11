<script setup lang="ts">

// ไว้กำหนด Meta ของหน้าเว็บ เช่น title, description, keyword รวมทั้ง layout ที่ใช้
definePageMeta({
    layout: 'auth',
})

</script>

<template>
    <div class="min-h-screen grid place-items-center p-4">
        <div class="relative w-full max-w-5xl  rounded-3xl shadow-lg overflow-hidden border border-gray-200">
            <!-- แบ่งซ้าย/ขวาด้วยกริด -->
            <div class="grid md:grid-cols-2">
                <!-- ฝั่งซ้าย (ตกแต่ง) -->
                <div class="hidden md:block">
                    <div class="h-full min-h-[28rem] w-full bg-gradient-to-b from-gray-100 to-gray-50"></div>
                </div>

                <!-- ฝั่งขวา: การ์ดฟอร์ม -->
                <div class="p-8 md:p-12 flex justify-center">
                    <div class="w-full max-w-md  rounded-3xl border border-gray-200 p-8 md:p-10">
                        <h1 class="text-3xl font-semibold text-center">Login your account!</h1>

                        <form class="mt-8 space-y-5">
                            <div>
                                <label class="block text-sm mb-2">Email</label>
                                <input type="email" autocomplete="email"
                                    class="w-full rounded-xl border border-gray-300 focus:border-gray-900 focus:ring-0 px-4 h-12"
                                    placeholder="Email" />
                            </div>

                            <div>
                                <div class="flex items-center justify-between mb-2">
                                    <label class="block text-sm">Password</label>
                                    <NuxtLink to="/forgot" class="text-xs underline">ลืมรหัสผ่าน?</NuxtLink>
                                </div>
                                <input type="password" autocomplete="current-password"
                                    class="w-full rounded-xl border border-gray-300 focus:border-gray-900 focus:ring-0 px-4 h-12"
                                    placeholder="Password" />
                            </div>

                            <button type="submit"
                                class="w-full h-12 rounded-xl border border-gray-900 hover:bg-gray-900 hover:text-white transition">
                                Login
                            </button>
                        </form>

                        <p class="mt-6 text-center text-sm">
                            ยังไม่มีสมาชิก?
                            <NuxtLink to="/sign-Up" class="underline">สมัครสมาชิก sign up</NuxtLink>
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped></style>
