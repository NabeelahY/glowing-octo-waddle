<template>
  <b-container>
    <h1>Services</h1>
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#ababab"
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <b-carousel-slide
        v-for="(service, index) in services"
        :key="index"
        caption="Service"
        :text="service.desc"
        :img-src="service.img"
      ></b-carousel-slide>
    </b-carousel>
  </b-container>
</template>

<script>
export default {
  name: "Service",
  data() {
    return {
      slide: 0,
      sliding: null,
      services: Array(3).fill({
        img: "https://picsum.photos/1024/480",
        desc: "Nulla vitae elit libero, a pharetra augue mollis interdum."
      })
    };
  },
  methods: {
    onSlideStart() {
      this.sliding = true;
    },
    onSlideEnd() {
      this.sliding = false;
    }
  }
};
</script>

<style scoped>
</style>