<template>
  <b-container>
    <h2>About Us</h2>
    <b-row>
      <b-col v-for="(section, index) in sections" :key="index" sm="12" md="4">
        <b-card class="text-center" :title="section.title">
          <b-icon :icon="section.icon"></b-icon>
          <b-card-text>{{section.desc}}</b-card-text>
        </b-card>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
  name: "about",
  data() {
    return {
      sections: [
        {
          title: "Coffee",
          icon: "view-stacked",
          desc:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus consequat sollicitudin nunc, a porttitor ipsum sollicitudin non. Donec sollicitudin posuere metus."
        },
        {
          title: "Tea",
          icon: "grid",
          desc:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus consequat sollicitudin nunc, a porttitor ipsum sollicitudin non. Donec sollicitudin posuere metus."
        },
        {
          title: "Chocolate",
          icon: "cup",
          desc:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus consequat sollicitudin nunc, a porttitor ipsum sollicitudin non. Donec sollicitudin posuere metus."
        }
      ]
    };
  }
};
</script>

<style scoped>
.row {
  margin: 30px 0;
}
</style>