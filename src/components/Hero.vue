<template>
  <b-container>
    <b-row class="text-center hero">
      <b-col class="mid" sm="12" md="4">
        <h1>Welcome to Site!</h1>
        <p>Leading market for all things luck</p>
        <b-button variant="info" href="#">More Info</b-button>
      </b-col>
      <b-col sm="12" md="6">
        <b-img fluid :src="image" alt="Image 1"></b-img>
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
.container {
  border-bottom: 1px solid;
  margin-bottom: 20px;
}
.hero {
  padding: 40px 0;
  margin: 40px 0;
}
.mid {
  flex-direction: column;
  align-self: center;
}

</style>
