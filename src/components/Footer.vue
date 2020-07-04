<template>
  <div class="footer">
    <p>{{time}} &copy; Made with Vue</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      time: new Date().getFullYear()
    };
  }
};
</script>

<style scoped>
.footer {
  background-color: #17a2b8;
  padding: 10px 0;
}
p {
  text-align: center;
  color: #fff;
}
</style>