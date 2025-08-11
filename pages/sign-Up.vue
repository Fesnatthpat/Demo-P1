<script setup lang="ts">

// ไว้กำหนด Meta ของหน้าเว็บ เช่น title, description, keyword รวมทั้ง layout ที่ใช้
definePageMeta({
    layout: 'auth',
})

</script>

<template>
    <div class="min-h-screen flex items-center justify-center p-4 sm:p-6 lg:p-10">
        <!-- การ์ดครอบฟอร์ม: ปรับกว้างตามจอ -->
        <div
            class="w-full max-w-md sm:max-w-lg md:max-w-xl lg:max-w-2xl xl:max-w-[900px] bg-white border border-gray-200 rounded-2xl shadow-lg">
            <div class="px-5 sm:px-8 md:px-10">
                <!-- หัวข้อ -->
                <h1 class="mt-8 text-2xl sm:text-3xl font-semibold text-center">Sign Up</h1>

                <!-- ฟอร์ม -->
                <form class="mt-8 space-y-6">
                    <!-- กริดฟิลด์: 1 คอลัมน์บนมือถือ, 2 คอลัมน์ตั้งแต่ sm ขึ้นไป -->
                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 sm:gap-5">
                        <div>
                            <label class="block text-sm mb-2">ชื่อ - สกุล</label>
                            <input type="text" autocomplete="name"
                                class="w-full rounded-xl border border-gray-300 focus:border-gray-900 focus:ring-0 px-4 h-12"
                                placeholder="ชื่อ - สกุล" />
                        </div>

                        <div>
                            <label class="block text-sm mb-2">Email</label>
                            <input type="email" autocomplete="email"
                                class="w-full rounded-xl border border-gray-300 focus:border-gray-900 focus:ring-0 px-4 h-12"
                                placeholder="Email" />
                        </div>

                        <div>
                            <label class="block text-sm mb-2">รหัสนักศึกษา/อาจารย์</label>
                            <input type="text"
                                class="w-full rounded-xl border border-gray-300 focus:border-gray-900 focus:ring-0 px-4 h-12"
                                placeholder="รหัสนักศึกษา/อาจารย์" />
                        </div>

                        <div>
                            <label class="block text-sm mb-2">Password</label>
                            <input type="password" autocomplete="new-password"
                                class="w-full rounded-xl border border-gray-300 focus:border-gray-900 focus:ring-0 px-4 h-12"
                                placeholder="Password" />
                        </div>

                        <div>
                            <label class="block text-sm mb-2">เบอร์โทรศัพท์</label>
                            <input type="tel" autocomplete="tel"
                                class="w-full rounded-xl border border-gray-300 focus:border-gray-900 focus:ring-0 px-4 h-12"
                                placeholder="012-3456-7890" />
                        </div>

                        <div>
                            <label class="block text-sm mb-2">ID - Line</label>
                            <input type="text"
                                class="w-full rounded-xl border border-gray-300 focus:border-gray-900 focus:ring-0 px-4 h-12"
                                placeholder="ID - Line" />
                        </div>
                    </div>

                    <!-- ปุ่ม: เต็มความกว้างบนมือถือ แคบลงบนจอใหญ่ -->
                    <div class="flex justify-center">
                        <button type="submit"
                            class="w-full sm:w-56 md:w-64 h-12 rounded-xl border border-gray-900 hover:bg-gray-900 hover:text-white transition">
                            Sign Up
                        </button>
                    </div>
                </form>

                <!-- เว้นระยะล่าง -->
                <div class="h-8"></div>
            </div>
        </div>
    </div>
</template>

<style scoped></style>
