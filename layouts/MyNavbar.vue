<template>
  <b-container fluid class="px-0">
    <b-navbar
      toggleable="lg"
      type="light"
      class="py-0"
      style="background-color: #f5f5f5"
    >
      <nuxt-link to="/" tag="b-navbar-brand">
        Docteur Gilbert Roux
      </nuxt-link>
      <b-navbar-toggle target="nav-collapse" />
      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <nuxt-link to="/cabinet" tag="b-nav-item" active-class="my-item">
            <div class="nav-link">
              Cabinet
            </div>
          </nuxt-link>
          <nuxt-link to="/soins" tag="b-nav-item" active-class="my-item">
            <div class="nav-link">
              Soins
            </div>
          </nuxt-link>
          <nuxt-link to="/accès" tag="b-nav-item" active-class="my-item">
            <div class="nav-link">
              Accès
            </div>
          </nuxt-link>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </b-container>
</template>

<script></script>

<style>
.navbar-brand:hover {
  cursor: pointer;
}
.nav-link:hover {
  cursor: pointer;
}
.my-item {
  background-color: #e8e8e8;
  transition: 500ms;
}
</style>
