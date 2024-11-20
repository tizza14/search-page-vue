<template>
    <nav class="fixed flex flex-row w-full justify-between pl-6 pr-6 min-h-16 items-center top-0">

        <div>
            <a href="#">
                <h1 class="text-lg text-orange-300">JiaBa沒</h1>
            </a>
        </div>

        <div class="inputs flex flex-row absolute left-40">

            <div class="inputCat px-4">
            <input type="text" name="inputCat" id="" placeholder="美食分類、餐廳" class="h-10  font-light">
            <i class="fa-solid fa-utensils text-orange-300"></i>
            </div>

            <div class="line"></div>

            <div class="inputPlace px-4">
            <input type="text" name="inputPlace" id="" placeholder="搜尋地點" class="h-10  font-light">
            <i class="fa-solid fa-location-dot text-orange-300"></i>
            </div>

            <div class="btn bg-orange-300">
            <button class="h-10 px-4 ">
                <i class="fa-solid fa-magnifying-glass text-white"></i>
            </button>
            </div>
        </div>

        <div class="rightSide flex flex-row items-center">
            <div class="p-3 text-sm text-gray-600 hover:bg-gray-200 rounded-md">
                <a href="#">發表食記</a>
            </div>

            <div class="rightSideLine"></div>

            <div class="p-3 text-sm text-gray-600 hover:bg-gray-200 rounded-md">
                <a href="#">專欄文章</a>
            </div>

            <div class="rightSideLine"></div>

            <div class="p-3 text-sm text-gray-600 hover:bg-gray-200 rounded-md">
                <a class="rankingList" href="#">排行榜</a>
                <ul class="ranking">
                    <li>週排行</li>
                    <li>月排行</li>
                </ul>
            </div>

            <div class="rightSideLine"></div>

            <div class="p-3 text-sm text-gray-600 hover:bg-gray-200 rounded-md">
                <a href="#">登入</a>
            </div>
        </div>
    </nav>
</template>

<style lang="css" scoped>
.line {
    border: 0.5px solid rgb(253,186,116);
}

.inputCat {
    border-radius: 5px 0 0 5px;
    box-shadow: rgba(0, 0, 0, 0.15) 0px 2px 18px 0px;
    ;
}

.inputPlace {
    box-shadow: rgba(0, 0, 0, 0.15) 0px 2px 18px 0px;
}

.btn {
    border-radius: 0 5px 5px 0;
    box-shadow: rgba(0, 0, 0, 0.15) 0px 2px 18px 0px; 
}

.rightSideLine {
    width: 1px;
    height: 27px;
    border-right: 1px solid black;
}

</style>