<template>
  <Header
    phone="+7 987 654 32-10"
  />
  <Main/>
</template>

<script>
import Header from '@/components/blocks/Header.vue'
import Main from '@/components/blocks/Main.vue'

export default {
  name: 'MainPage',
  components: {
    Header,
    Main
  }
}
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap');
</style>
