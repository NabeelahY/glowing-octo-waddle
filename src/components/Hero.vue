<template>
  <b-container>
    <b-row class="text-center hero">
      <b-col cols="6">
        <b-img fluid :src="image" alt="Image 1"></b-img>
      </b-col>
      <b-col class="mid">
        <h1>Welcome to Site!</h1>
        <p>Leading market for all things luck</p>
        <b-button variant="info" href="#">More Info</b-button>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import image from "../assets/hero.svg";
export default {
  name: "Hero",
  data() {
    return {
      links: ["Home", "Team", "Services", "Contact"],
      image: image
    };
  }
};
</script>

<style scoped>
.hero {
  padding: 30px 0;
}
.mid {
  flex-direction: column;
  align-self: center;
}
</style>
