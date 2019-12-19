<template>
  <div
    :style="{ backgroundImage: `url(${bgUrl})` }"
    class="banner
    d-flex
    align-items-center
    flex-column"
  >
    <div
      class="text-container
      d-flex
      align-items-center
      justify-content-center
      flex-column
      text-center"
    >
      <h1>{{ title }}</h1>
      <h4>{{ subtitle }}</h4>
    </div>
  </div>
</template>

<script>
export default {
  props: ['title', 'subtitle', 'bgUrl', 'text']
}
</script>
