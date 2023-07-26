<template>
  <div class="w-full min-h-screen bg-gray-200">
    <div class="w-full max-w-sm min-h-screen mx-auto bg-white">
        <header class="relative">
            <img class="h-48 w-full" src="https://st2.depositphotos.com/38693846/43772/i/450/depositphotos_437728098-stock-photo-sukiyaki-japanese-food-shabu-shabu.jpg">
            <div class="absolute mx-auto left-32 top-32 rounded-full border-4 border-white shadow-xl">
                <img class="h-32 w-32 rounded-full " src="https://scontent.fbkk22-8.fna.fbcdn.net/v/t39.30808-6/305705178_101148912750846_1897431402344675181_n.jpg?_nc_cat=108&cb=99be929b-59f725be&ccb=1-7&_nc_sid=09cbfe&_nc_eui2=AeFH3vJMluF__zTwmdcZlM19GKZqIgUyDrkYpmoiBTIOuSTXge_cNjaI7yZjjptHkRqXrb2dgtusufpRlRI00Pyd&_nc_ohc=vc3zx-LgVXAAX-XA_pX&_nc_zt=23&_nc_ht=scontent.fbkk22-8.fna&oh=00_AfCzI5CW6FJ6f3Wc6UoIvaumyZjPdwYDJoz-2tnTieTxYA&oe=64C694FC">
            </div>
        </header>
        <div class="flex flex-col items-center mt-24 text-gray-600">
            <div class="font-bold text-xl ">เรียวตะชาบู</div>
            <div class="text-sm">Ryota Shabu Robinson</div>
            <div class="flex flex-wrap py-4">
                <div class="border-r-2 border-gray-300 px-3">
                    โต๊ะ<span class="font-bold"> 22</span>
                </div>
                <div class="px-3">
                    คุณ:<span class="font-bold">A</span>
                </div>
            </div>
        </div>
        <div class="">
            <div class="flex flex-wrap justify-between bg-gray-100 mx-5 my-2 py-4 px-4 rounded-xl">
                <div>
                    <div class="font-semibold text-gray-700">Buffet 199 + refill 39</div>
                    <div><span class="text-gray-600">2 ท่าน</span></div>
                </div>
                <div class="text-sm text-gray-400 text-right">
                    <div>18:47 - 20:37</div>
                    <div>เวลาทาน : <span>110 นาที</span></div>
                </div>
            </div>
            <button type="button" class="w-full">
                <div class=" flex flex-wrap items-center justify-between bg-sky-400 mx-5 my-3 py-4 px-4 rounded-xl">
                <div class="text-white">สั่งอาหาร</div>
                <div class="w-10 h-10 bg-white rounded-full left-72 top-3 shadow-lg">
                        <svg class="w-6 h-6 mt-2 ml-2  dark:text-sky-400" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 8 14">
                            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m1 13 5.7-5.326a.909.909 0 0 0 0-1.348L1 1"/>
                        </svg>
                </div>           
            </div>
            </button>
        </div>

        <div class="flex mx-3">
            <a href="#" class="flex flex-col items-center justify-center w-28 h-28 mx-1.5 my-3 bg-white rounded-xl shadow-lg text-gray-500 text-sm">
                <img class="h-14 my-1" src="../asset/icons8-list-64.png">
                <span>รายการที่สั่ง</span>
            </a>
            <a href="#" class="flex flex-col items-center justify-center w-28 h-28 mx-1.5 my-3 bg-white rounded-xl shadow-lg text-gray-500 text-sm">
                <img class="h-14 my-1" src="../asset/icons8-waiter-64.png">
                <span>เรียกพนักงาน</span>
            </a>
            <a href="#" class="flex flex-col items-center justify-center w-28 h-28 mx-1.5 my-3 bg-white rounded-xl shadow-lg text-gray-500 text-sm">
                <img class="h-14 my-1" src="../asset/icons8-qr-64.png">
                <span>แชร์ QR ให้เพื่อน</span>
            </a>
        </div>
    </div>
  </div>
</template>
