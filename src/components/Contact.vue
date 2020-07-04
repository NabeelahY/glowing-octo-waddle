<template>
  <b-container>
    <div class="contact">
      <h2>Contact Us</h2>
      <b-form-group>
        <b-form-input type="text" placeholder="Enter Name" trim></b-form-input>
      </b-form-group>
      <b-form-group>
        <b-form-input type="email" placeholder="Enter Email" trim></b-form-input>
      </b-form-group>
      <b-form-group>
        <b-form-textarea placeholder="What would you like to enquire about?"></b-form-textarea>
      </b-form-group>
      <b-button type="submit" block variant="outline-info">Submit</b-button>
    </div>
  </b-container>
</template>

<script>
export default {
  name: "Conatct"
};
</script>

<style scoped>
.contact {
  margin: 40px 0;
  padding: 20px 0;
  border-top: 1px solid;
}
h2 {
  margin-bottom: 20px;
}

textarea {
  resize: none;
}
</style>