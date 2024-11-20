<template>
  <div class="pt-32">
    <Navbar />
    <FilterBar />
    <div class="flex flex-col lg:flex-row">
      <!-- 餐廳列表 -->
      <div class="w-full lg:w-1/2 p-4">
        <RestaurantCard v-for="(restaurant, index) in restaurants" :key="index" :restaurant="restaurant" />
      </div>
      <!-- 地圖 -->
      <div class="w-full lg:w-1/2 h-96 lg:h-screen">
        <MapView />
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import FilterBar from './components/FilterBar.vue';
import RestaurantCard from './components/RestaurantCard.vue';
import MapView from './components/MapView.vue';

export default {
  components: {
    Navbar,
    FilterBar,
    RestaurantCard,
    MapView,
  },
  data() {
    return {
      restaurants: [
        {
          name: '九州拉麵',
          description: '正宗日式拉麵，濃郁湯頭。',
          image: 'https://via.placeholder.com/150',
        },
        {
          name: '東京咖啡',
          description: '舒適空間，頂級咖啡豆。',
          image: 'https://via.placeholder.com/150',
        },
        {
          name: '東京咖啡',
          description: '舒適空間，頂級咖啡豆。',
          image: 'https://via.placeholder.com/150',
        },
        {
          name: '東京咖啡',
          description: '舒適空間，頂級咖啡豆。',
          image: 'https://via.placeholder.com/150',
        },
        {
          name: '東京咖啡',
          description: '舒適空間，頂級咖啡豆。',
          image: 'https://via.placeholder.com/150',
        },
        {
          name: '東京咖啡',
          description: '舒適空間，頂級咖啡豆。',
          image: 'https://via.placeholder.com/150',
        },
      ],
    };
  },
};
</script>