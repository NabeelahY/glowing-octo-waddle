<template>
  <div class="teams" id="Team">
    <b-container>
      <h2>Meet Our Team</h2>
      <b-row>
        <b-col v-for="(team, index) in teams" :key="index" sm="12" md="4">
          <b-card
            class="overflow-hidden"
            :img-src="team.img"
            img-alt="Image"
            img-top
            style="max-width: 540px;"
            :key="index"
          >
            <b-card-text>{{team.position}}</b-card-text>
          </b-card>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import avatar from "../assets/avatar.svg";
export default {
  name: "Team",
  data() {
    return {
      teams: [
        { name: "John", img: avatar, position: "Software Engineer" },
        { name: "Jane", img: avatar, position: "Software Engineer" },
        { name: "Bob", img: avatar, position: "Software Engineer" }
      ]
    };
  }
};
</script>

<style scoped>
.teams {
  margin: 20px 0;
}
</style>