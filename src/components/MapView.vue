<template>
    <div class="w-full h-full">
        <div id="map" class="h-full w-full"></div>
    </div>
</template>

<script>
import { onMounted, ref } from "vue";

export default {
    name: "MapView",
    setup() {
        const map = ref(null);
        const restaurants = [
            {
                id: 1,
                name: "九份美食拉麵",
                lat: 25.10898,
                lng: 121.84351,
            },
            {
                id: 2,
                name: "阿婆豆花",
                lat: 25.1085,
                lng: 121.8440,
            },
            {
                id: 3,
                name: "山海美景咖啡廳",
                lat: 25.1092,
                lng: 121.8428,
            },
        ];

        onMounted(() => {
            loadMap();
        });

        const loadMap = () => {
            const google = window.google;

            // 初始化地圖
            map.value = new google.maps.Map(document.getElementById("map"), {
                center: { lat: 25.10898, lng: 121.84351 }, // 地圖中心點
                zoom: 15,
            });

            // 為每個餐廳新增標記
            restaurants.forEach((restaurant) => {
                new google.maps.Marker({
                    position: { lat: restaurant.lat, lng: restaurant.lng },
                    map: map.value,
                    title: restaurant.name,
                });
            });
        };

        return { restaurants };
    },
};
</script>

<style scoped>
#map {
    height: 100%;
    width: 100%;
}
</style>