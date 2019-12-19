<template>
  <div
    id="full-card"
    class="p-0 m-3 text-center col-12 col-sm-6 col-md-3 col-lg-3"
    style="max-width: 25rem;"
  >
    <b-card
      :title="title"
      img-src="https://picsum.photos/600/300/?image=25"
      img-alt="Image"
      img-top
      tag="article"
    >
      <b-card-text>
        Some quick example text to build on the card title.
      </b-card-text>
      <b-button href="#" variant="primary">Go somewhere</b-button>
    </b-card>
  </div>
</template>

<script>
export default {
  props: ['title', 'path']
}
</script>

<style scoped>
#full-card {
  transition: 500ms;
}
#full-card:hover {
  transform: translate(-1px, -3px);
  box-shadow: 6px 7px 5px rgba(0, 0, 0, 0.1);
  transition: 1s;
}
</style>
