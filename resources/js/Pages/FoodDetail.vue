<script setup></script>

<template>
    <div class="w-full min-h-screen bg-gray-200">
        <div class="w-full max-w-sm min-h-screen mx-auto bg-white">
            <div
                class="relative flex items-center justify-center w-full h-50% border-b-2 border-gray-100 shadow"
            >
                <div>
                    <img
                        class="w-full h-full drop-shadow-xl rounded-xl"
                        src="../asset/img_page_5.png"
                        alt=""
                    />
                </div>
                <button class="absolute text-xl text-white w-10 h-10 font-bold top-2 left-2 border-2 border-gray-800 bg-gray-800 rounded-full">
                    X
                </button>
            </div>
            <div class="w-full max-w-sm mx-auto border-t-2 border-gray-100">
                <div class="items-center justify-center p-4 h-3/6">
                    <div class="font-bold text-lg">1.2 สามชั้น Belly Pork.</div>
                    <div class="font-bold text-lg">
                        <span>ข้อความเพิ่มเติม</span>
                    </div>
                    <div class="text-l ml-2">
                        คุณสามารถใส่ข้อความเพิ่มเติมได้ที่นี่ เช่น อาหารที่แพ้
                    </div>
                    <textarea
                        class="p-2.5 w-full h-36 text-l mt-3 text-gray-900 bg-gray-50 rounded-lg border border-gray-300 focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
                        placeholder="ตัวอย่างไม่ใส่ผงชูรส"
                    ></textarea>
                </div>
            </div>
            <div
                class="flex justify-between w-full max-w-sm mx-auto border-t-2 border-gray-100 h-auto"
            >
                <button
                    @click="decrease"
                    class="flex w-1/12 h-1/6 mt-8 mx-auto border-2 border-blue-500 text-blue-500 rounded-full"
                >
                    <span class="items-center justify-center ml-2.5 text-xl"
                        >-</span
                    >
                </button>
                <span class="mt-8 p-1">{{ quantity }}</span>
                <button
                    @click="increase"
                    class="flex w-1/12 h-1/6 mt-8 mx-auto border-2 border-blue-500 text-blue-500 rounded-full"
                >
                    <span class="items-center justify-center ml-2.5 text-xl"
                        >+</span
                    >
                </button>
                <button
                    class="flex items-center justify-center w-7/12 p-3 mt-5 mx-auto text-xl font-bold text-white bg-blue-400 border-2 border-blue-400 rounded-xl"
                >
                    <span class="">เพิ่มลงตะกร้า</span>
                </button>
            </div>
        </div>
    </div>
</template>
<script>
import { ref } from "vue";

export default {
    setup() {
        // สร้างตัวแปร ref เพื่อเก็บค่าจำนวนสินค้า
        const quantity = ref(0);

        // ฟังก์ชันเพิ่มจำนวนสินค้า
        const increase = () => {
            quantity.value++;
            updateQuantity();
        };

        // ฟังก์ชันลดจำนวนสินค้า
        const decrease = () => {
            if (quantity.value > 0) {
                quantity.value--;
                updateQuantity();
            }
        };

        // อัปเดตจำนวนสินค้าที่แสดงบนหน้าจอ
        const updateQuantity = () => {
            quantityElement.textContent = quantity.value;
        };

        return {
            quantity,
            increase,
            decrease,
        };
    },
};
</script>
