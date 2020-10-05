<template>
  <div class="trip_picture">
    <div class="image1 image">
      <router-link to="/">
        <div class="image_1 image-1"></div>
        <div class="text">{{ place1 }}, {{ province1 }}</div>
      </router-link>
    </div>
    <div class="image2 image">
      <router-link to="/">
        <div class="image_2 image-1"></div>
        <div class="text">{{ place2 }}, {{ province2 }}</div>
      </router-link>
    </div>
    <div class="image3 image">
      <router-link to="/">
        <div class="image_3 image-1"></div>
        <div class="text">{{ place3 }}, {{ province3 }}</div>
      </router-link>
    </div>
    <div class="image4 image">
      <router-link to="/">
        <div class="image_4 image-1"></div>
        <div class="text">{{ place4 }}, {{ province4 }}</div>
      </router-link>
    </div>
  </div>
</template>


<script>
export default {
  name: "NextTripPage",
  props: {
    place1: String,
    province1: String,

    place2: String,
    province2: String,

    place3: String,
    province3: String,

    place4: String,
    province4: String,
  },
};
</script>

<style scoped>
.trip_picture {
  width: 75%;
  height: 27.8vw;
  margin-left: 13%;
  margin-top: 2vw;
  display: flex;
}
.image {
  width: 24%;
  height: 19.8vw;
  margin-top: 3vw;
  margin-left: 8px;
  background-color: white;
}
.image-1 {
  width: 100%;
  height: 16vw;
  background-size: cover;
  background-position: 30%;
}
.image-1:hover {
  opacity: 0.8;
}
.image_1 {
  background-image: url("./assets_element/koh-thansur.jpg");
}
.image_2 {
  background-image: url("./assets_element/Koh-Rong-Samloem.jpg");
}
.image_3 {
  background-image: url("./assets_element/bengYakLoum.jpg");
}
.image_4 {
  background-image: url("./assets_element//Ankor_Wat.jpg");
}
.text {
  width: 100%;
  height: 3.75vw;
  padding-top: 0.9vw;
  /* margin-top: 10px; */
  font-size: 1.25vw;
}
a.router-link-active {
  color: black;
  text-decoration: none;
}
a.router-link-active:hover {
  text-decoration: underline;
}
</style>