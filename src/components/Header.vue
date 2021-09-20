<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="info" style="padding: 10px 10px">
      <b-navbar-brand href="#">Vue-Samurai</b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ms-auto">
          <b-nav-item to="/">Home</b-nav-item>
          <b-nav-item to="/about">Sobre</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {};
</script>
