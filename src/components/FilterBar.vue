<template>
    <div class="px-6 py-2 fixed top-16 flex flex-row">
        <div class="flex flex-col">
            <div class="px-3 text-base text-gray-700">
                <!-- 跟navbar搜尋篩選做變化 -->
                <h3>台灣『美食餐廳』 | 精選TOP 15間熱門店家</h3>
            </div>
            <div class="flex flex-row text-sm  text-gray-600">
                <div class="px-3">
                    <a href="#">台灣</a>
                </div>

                <div>
                    <i class="fa-solid fa-chevron-right"></i>
                </div>

                <div class="px-3">
                    <span>所有餐廳</span>
                </div>
            </div>
        </div>
        <div class="filters flex flex-row">
            <div class="cat bg-orange-300 mr-3.5">
                <ul>
                    <li>評分最高</li>
                    <li>最新餐廳</li>
                    <li>最高人氣</li>
                </ul>
            </div>
            <div class="consume bg-orange-300 mr-3.5">平均消費
                <ul>
                    <li>不選擇</li>
                    <li>150以內</li>
                    <li>150~600</li>
                    <li>600~1200</li>
                    <li>1200以上</li>
                </ul>
            </div>
            <div class="checkBoxs">
                <input type="checkbox" name="open">營業中</input>
                <input type="checkbox" name="takeOut">外帶外送</input>

            </div>
        </div>
    </div>
</template>