<template>
  <b-navbar toggleable="lg" type="dark" variant="info" fixed="top">
    <b-navbar-brand v-scroll-to="'#home'" href="#">Vue Site</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav v-for="(link, index) in links" :key="index">
        <b-nav-item v-scroll-to:link="'#' + link">{{ link }}</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {
      links: ["About", "Services", "Team", "Contact"]
    };
  }
};
</script>
