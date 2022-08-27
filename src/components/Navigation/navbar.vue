<template>
  <b-navbar toggleable type="dark" variant="dark" class="px-4">
    <b-navbar-brand href="#">
      <b-icon icon="house"> </b-icon>
      <span>Tony Monier</span></b-navbar-brand
    >

    <b-navbar-toggle
      target="navbar-toggle-collapse"
      style="width: 56px; height: 40px"
    >
      <template #default="{ expanded }">
        <b-icon v-if="expanded" icon="x-lg"></b-icon>
        <b-icon v-else class="navbar-toggler-icon"></b-icon>
      </template>
    </b-navbar-toggle>

    <b-collapse id="navbar-toggle-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item class="mx-auto" href="#">About</b-nav-item>
        <b-nav-item class="mx-auto" href="#">Mission</b-nav-item>
        <b-nav-item class="mx-auto" href="#">Vision</b-nav-item>
        <b-nav-item class="mx-auto" href="#">Contact Us</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>
<script>
// @ is an alias to /src
export default {
  name: "navbar",
  data() {
    return {
      expanded: false,
    };
  },
};
</script>
<style lang="scss">
.navbar-toggler:focus {
  text-decoration: none;
  outline: 0;
  box-shadow: 0 0 0 0;
}
</style>
