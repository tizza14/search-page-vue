<template>
    <div class="border rounded-lg shadow-lg overflow-hidden">
        <!-- 圖片 -->
        <img :src="restaurant.image" :alt="restaurant.name" class="w-full h-40 object-cover" />

        <!-- 資訊 -->
        <div class="p-4">
            <h2 class="text-lg font-bold mb-2">{{ restaurant.name }}</h2>
            <p class="text-sm text-gray-500 mb-2">{{ restaurant.address }}</p>

            <!-- 評價與評論數 -->
            <div class="flex items-center text-yellow-500 text-sm">
                <span class="mr-2">⭐ {{ restaurant.rating }}</span>
                <span class="text-gray-500">({{ restaurant.reviews }} 則評論)</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            // 靜態資料
            restaurant: {
                id: 1,
                name: "九份阿婆芋圓",
                address: "新北市瑞芳區輕便路10號",
                image: "https://via.placeholder.com/300x200.png?text=九份阿婆芋圓",
                rating: 4.7,
                reviews: 132,
            },
        };
    },
};
</script>

<style scoped></style>