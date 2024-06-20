<script setup>
import ProductDetail from "./components/productDetails.vue";
import Novosti from "./components/Novosti.vue";
import VideoNovosti from "./components/VideoNovosti.vue";
import { ref } from "vue";

const data = ref([
  {
    id: 1,
    name: "POLO Рубашка",
    price: 49900,
    sku: 685813,
    posadka: "высокая посадка",
    rating: "* * * * *",
    kroy: "средняя посадка",
    sostav: "100% хлопок",
    vIzbranniy: false,
    mainImage: "/main.png",
    img1: "/1.png",
    img2: "/2.png",
    img3: "/3.png",
    img4: "/4.png",
    description:
      "Рубашка с контрастным дизайном Свитшот из мягкого футера. Довольно свободная модель с заниженной линией плеча. Рельефная трикотажная резинка по горловине, низу рукавов и нижнему краю. ",
  },
]);
</script>

<template>
  <div>
    <ProductDetail :product="data[0]" />
    <Novosti />
    <VideoNovosti />
  </div>
</template>

<style scoped></style>
