<script setup lang="ts">
</script>

<template>
    <div class="min-h-screen px-4 sm:px-6 lg:px-10 py-6 sm:py-10">
        <!-- กรอบหลัก -->
        <div class="mx-auto w-full max-w-6xl rounded-3xl border-2 border-blue-600 p-4 sm:p-8 md:p-12">
            <!-- หัวข้อ -->
            <h1 class="text-center font-bold text-2xl sm:text-3xl md:text-4xl">บัณฑิตนิพนธ์</h1>

            <!-- แถวค้นหา + ตัวกรอง -->
            <div
                class="mt-6 sm:mt-8 grid grid-cols-1 md:grid-cols-[1fr_auto_auto] gap-3 sm:gap-4 md:gap-6 items-center">
                <!-- ค้นหา -->
                <div class="relative">
                    <input type="text" placeholder="ค้นหาโครงงาน..."
                        class="w-full h-12 sm:h-14 rounded-full border border-gray-400 pl-5 pr-12 text-base sm:text-lg placeholder:text-gray-700" />
                    <button type="button" aria-label="ค้นหา" class="absolute right-3 top-1/2 -translate-y-1/2 p-2">
                        <!-- ไอคอนแว่นขยาย (SVG) -->
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="h-5 w-5 sm:h-6 sm:w-6"
                            fill="none" stroke="currentColor" stroke-width="1.5">
                            <circle cx="11" cy="11" r="7"></circle>
                            <path d="m20 20-3.5-3.5" stroke-linecap="round"></path>
                        </svg>
                    </button>
                </div>

                <!-- ปีการศึกษา -->
                <div class="relative">
                    <select
                        class="h-12 sm:h-14 w-full md:w-56 rounded-xl border border-gray-900 pl-4 pr-10 appearance-none bg-white">
                        <option selected>ปีการศึกษา</option>
                        <option>2568</option>
                        <option>2567</option>
                        <option>2566</option>
                    </select>
                    <!-- ไอคอนลูกศร -->
                    <svg class="pointer-events-none absolute right-3 top-1/2 -translate-y-1/2 h-5 w-5"
                        xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd"
                            d="M5.23 7.21a.75.75 0 0 1 1.06.02L10 10.94l3.71-3.71a.75.75 0 1 1 1.06 1.06l-4.24 4.24a.75.75 0 0 1-1.06 0L5.21 8.29a.75.75 0 0 1 .02-1.08z"
                            clip-rule="evenodd" />
                    </svg>
                </div>

                <!-- หมวดหมู่โครงงาน -->
                <div class="relative">
                    <select
                        class="h-12 sm:h-14 w-full md:w-64 rounded-xl border border-gray-900 pl-4 pr-10 appearance-none bg-white">
                        <option selected>หมวดหมู่โครงงาน</option>
                        <option>ทั้งหมด</option>
                        <option>เว็บไซต์</option>
                        <option>โมบายแอป</option>
                        <option>AI / Data</option>
                    </select>
                    <svg class="pointer-events-none absolute right-3 top-1/2 -translate-y-1/2 h-5 w-5"
                        xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd"
                            d="M5.23 7.21a.75.75 0 0 1 1.06.02L10 10.94l3.71-3.71a.75.75 0 1 1 1.06 1.06l-4.24 4.24a.75.75 0 0 1-1.06 0L5.21 8.29a.75.75 0 0 1 .02-1.08z"
                            clip-rule="evenodd" />
                    </svg>
                </div>
            </div>

            <!-- กริดการ์ด 3 คอลัมน์ (2 แถว) -->
            <div class="mt-8 grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- การ์ดโครงงานตัวอย่าง -->
                <div class="rounded-xl border border-blue-500 p-4 flex flex-col">
                    <h3 class="font-semibold text-lg">ระบบจัดการหอพัก</h3>
                    <p class="mt-2 text-sm text-gray-600 flex-grow">
                        เว็บแอปพลิเคชันสำหรับจัดการข้อมูลผู้เช่า การชำระค่าเช่า และแจ้งซ่อมออนไลน์
                    </p>
                    <button
                        class="mt-4 self-start px-4 py-2 rounded-lg border border-gray-900 hover:bg-gray-900 hover:text-white transition text-sm">
                        ดูรายละเอียด
                    </button>
                </div>

                <div class="rounded-xl border border-blue-500 p-4 flex flex-col">
                    <h3 class="font-semibold text-lg">ระบบจองห้องประชุม</h3>
                    <p class="mt-2 text-sm text-gray-600 flex-grow">
                        แอปพลิเคชันจองห้องประชุมแบบออนไลน์ รองรับการอนุมัติและแจ้งเตือนผ่านอีเมล
                    </p>
                    <button
                        class="mt-4 self-start px-4 py-2 rounded-lg border border-gray-900 hover:bg-gray-900 hover:text-white transition text-sm">
                        ดูรายละเอียด
                    </button>
                </div>

                <div class="rounded-xl border border-blue-500 p-4 flex flex-col">
                    <h3 class="font-semibold text-lg">ระบบติดตามงานซ่อมบำรุง</h3>
                    <p class="mt-2 text-sm text-gray-600 flex-grow">
                        ระบบบันทึกและติดตามสถานะงานซ่อมบำรุงอุปกรณ์ พร้อมรายงานสรุปประจำเดือน
                    </p>
                    <button
                        class="mt-4 self-start px-4 py-2 rounded-lg border border-gray-900 hover:bg-gray-900 hover:text-white transition text-sm">
                        ดูรายละเอียด
                    </button>
                </div>

                <div class="rounded-xl border border-blue-500 p-4 flex flex-col">
                    <h3 class="font-semibold text-lg">แพลตฟอร์มเรียนออนไลน์</h3>
                    <p class="mt-2 text-sm text-gray-600 flex-grow">
                        ระบบคอร์สออนไลน์พร้อมการบ้าน ควิซ และติดตามความก้าวหน้าของผู้เรียน
                    </p>
                    <button
                        class="mt-4 self-start px-4 py-2 rounded-lg border border-gray-900 hover:bg-gray-900 hover:text-white transition text-sm">
                        ดูรายละเอียด
                    </button>
                </div>

                <div class="rounded-xl border border-blue-500 p-4 flex flex-col">
                    <h3 class="font-semibold text-lg">ระบบบริหารจัดการร้านอาหาร</h3>
                    <p class="mt-2 text-sm text-gray-600 flex-grow">
                        จัดการออเดอร์ โต๊ะอาหาร และสต๊อกวัตถุดิบ พร้อมสรุปยอดขายรายวัน
                    </p>
                    <button
                        class="mt-4 self-start px-4 py-2 rounded-lg border border-gray-900 hover:bg-gray-900 hover:text-white transition text-sm">
                        ดูรายละเอียด
                    </button>
                </div>

                <div class="rounded-xl border border-blue-500 p-4 flex flex-col">
                    <h3 class="font-semibold text-lg">ระบบติดตามการส่งพัสดุ</h3>
                    <p class="mt-2 text-sm text-gray-600 flex-grow">
                        เว็บแอปติดตามสถานะพัสดุและแจ้งเตือนเมื่อถึงปลายทาง รองรับหลายบริษัทขนส่ง
                    </p>
                    <button
                        class="mt-4 self-start px-4 py-2 rounded-lg border border-gray-900 hover:bg-gray-900 hover:text-white transition text-sm">
                        ดูรายละเอียด
                    </button>
                </div>
            </div>

        </div>
    </div>
</template>

<style scoped></style>
