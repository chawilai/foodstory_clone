<script setup></script>

<template>
    <div class="w-full min-h-screen bg-gray-200">
        <div class="w-full max-w-sm min-h-screen mx-auto bg-white">
            <div
                class="relative flex items-center justify-center w-full h-24 border-b-2 border-gray-100 shadow"
            >
                <div class="absolute text-xl font-bold top-9 left-5">X</div>
                <div class="text-xl font-bold">ตากร้่า</div>
            </div>
            <div
                v-for="item in 10"
                class="flex items-center justify-between p-3 border-b-2 border-gray-200"
            >
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
                            <div>
                                <button
                                    @click="isEditing = true"
                                    class="text-blue-600 text-left"
                                >
                                    แก้ไข
                                </button>
                                <div v-if="isEditing">
                                    <div class="bg-white rounded-lg shadow-md">
                                        <input
                                            v-model="editText"
                                            @blur="saveEdit"
                                            @keyup.enter="saveEdit"
                                            class="border border-blue-600 p-2 rounded-lg"
                                        />
                                        <button
                                            class="ml-3 border border-blue-600 p-2 rounded-lg"
                                        >
                                            ยืนยันแก้ไข
                                        </button>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <!-- ล่าง -->
                    <div class="mt-4 text-sm text-gray-400">สั่งโดย: A</div>
                </div>
                <div class="flex">
                    <button
                        @click="decrease"
                        class="flex mt-7 border-2 px-2 border-blue-500 text-blue-500 rounded-full"
                    >
                        <span class="items-center justify-center text-xl mt-0.5"
                            >-</span
                        >
                    </button>
                    <span class="mt-8 p-1">{{ quantity }}</span>
                    <button
                        @click="increase"
                        class="flex mt-7 border-2 px-2 border-blue-500 text-blue-500 rounded-full"
                    >
                        <span class="items-center justify-center text-xl mt-0.5"
                            >+</span
                        >
                    </button>
                </div>
            </div>

            <div
                class="fixed bottom-0 w-full max-w-sm mx-auto border-t-2 border-gray-100 h-36 bg-white"
            >
                <div
                    class="flex items-center justify-between p-4 text-lg font-bold"
                >
                    <div>ทั้งหมด 10 รายการ</div>
                    <div>฿ 0.00 <span></span></div>
                </div>
                <button
                    class="flex items-center justify-center w-11/12 p-3 mx-auto text-xl font-bold bg-blue-400 text-white border-2 border-blue-400 rounded-xl"
                >
                    <span class="mr-2">สั่งทั้งหมด</span>
                </button>
            </div>
        </div>
    </div>
</template>
<script>
import { ref } from "vue";

export default {
    setup() {

        const quantity = ref(0);
        const increase = () => {
            quantity.value++;
            updateQuantity();
        }

        const decrease = () => {
            if (quantity.value > 0) {
                quantity.value--;
                updateQuantity();
            }
        };

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

