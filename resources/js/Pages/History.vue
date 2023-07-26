<script setup></script>

<template>
    <div class="w-full min-h-screen bg-gray-200">
    <div class="w-full max-w-sm min-h-screen mx-auto bg-white">
        <div
            class="relative flex items-center justify-center w-full h-24 border-b-2 border-gray-100 shadow"
        >
            <div class="absolute text-xl font-bold top-9 left-5">X</div>
            <div class="text-xl font-bold">รายการที่สั่ง</div>
        </div>
        <div class="flex items-center justify-between p-3 border-b-2 border-gray-200">
            <div class="">
                <!-- บน -->
                <div class="flex items-center gap-x-2">
                    <!-- รูป -->
                    <div>
                        <img
                            class="w-24 h-24 drop-shadow-xl rounded-xl"
                            src="../asset/pork.png"
                            alt=""
                        />
                    </div>
                    <!-- ข้อมูล -->
                    <div class="flex flex-col gap-y-4">
                        <div>1.2 สามชั้น Belly Pork.</div>
                        <div>x 3</div>
                    </div>
                </div>
                <!-- ล่าง -->
                <div class="mt-4 text-sm text-gray-400">สั่งโดย: A</div>
            </div>
            <!-- ssdf -->
            <div class="flex items-center justify-center">
                <span
                    class="px-4 py-2 text-xs text-white bg-orange-400 rounded-xl"
                >
                    กำลังทำ
                </span>
            </div>
        </div>
        <div class="flex items-center justify-between p-3 border-b-2 border-gray-200">
            <div class="">
                <!-- บน -->
                <div class="flex items-center gap-x-2">
                    <!-- รูป -->
                    <div>
                        <img
                            class="w-24 h-24 drop-shadow-xl rounded-xl"
                            src="../asset/pork.png"
                            alt=""
                        />
                    </div>
                    <!-- ข้อมูล -->
                    <div class="flex flex-col gap-y-4">
                        <div>1.2 สามชั้น Belly Pork.</div>
                        <div>x 3</div>
                    </div>
                </div>
                <!-- ล่าง -->
                <div class="mt-4 text-sm text-gray-400">สั่งโดย: A</div>
            </div>
            <div class="flex items-center justify-center">
                <button
                    class="px-4 py-2 text-xs text-white bg-orange-400 rounded-xl"
                >
                    กำลังทำ
                </button>
            </div>
        </div>
        <div class="fixed bottom-0 w-full max-w-sm mx-auto border-t-2 border-gray-100 h-36">
            <div
                class="flex items-center justify-between p-4 text-lg font-bold"
            >
                <div>23 รายการ</div>
                <div>฿ 0.00 <span>%</span></div>
            </div>
            <button
                class="flex items-center justify-center w-11/12 p-3 mx-auto text-xl font-bold text-blue-400 border-2 border-blue-400 rounded-xl"
            >
                <span class="mr-2">X</span>บิลค่าอาหาร
            </button>
        </div>
    </div>
    </div>
</template>
