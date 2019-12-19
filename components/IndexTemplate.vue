<template>
  <div
    class="banner
    d-flex
    align-items-center
    flex-column"
    style="background-image: url('https://picsum.photos/id/1056/3988/2720') "
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
      <h4>{{ subtitlea }}</h4>
      <h4>{{ subtitleb }}</h4>
    </div>
    <div id="cards-container" class="rounded">
      <MyCard v-for="card in cards" to="card.path" :title="card.cardTitle" />
    </div>
  </div>
</template>

<script>
import MyCard from '../components/MyCard.vue'

export default {
  components: {
    MyCard
  },
  data() {
    return {
      title: 'Cabinet du docteur Gilbert Roux',
      subtitlea: 'Chirurgien Dentiste à Marseille,',
      subtitleb: 'Spécialisé en implantologie et parodontologie',
      cards: [
        { cardTitle: 'Cabinet', path: '/cabinet' },
        { cardTitle: 'Implantologie', path: '/cabinet' },
        { cardTitle: 'Parodontologie', path: '/cabinet' },
        { cardTitle: 'Esthétique', path: '/cabinet' }
      ]
    }
  }
}
</script>

<style>
#cards-container {
  background-color: rgba(255, 255, 255, 1);
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
@media (width > 768px) {
  #cards-container {
  }
}
</style>
