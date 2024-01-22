<template>
  <main class="main">
    <div class="books">
        <Card
          name="Skyrim. История создания великой игры"
          autor="Франк Экстанази"
          :preview="require('@/assets/images/image_1.svg')"
        />
        <Card
          name="Поисковое продвижение сайтов"
          autor="Сергей Анисимов"
          :preview="require('@/assets/images/image_2.svg')"
        />
        <Card
          name="Английский для дизайнеров"
          autor="Татьяна Магарина"
          :preview="require('@/assets/images/image_3.svg')"
        />
        <Card
          name="Дизайн и цвет. Практикум"
          autor="Шон Адамс"
          :preview="require('@/assets/images/image_4.svg')"
        />
    </div>
  </main>
</template>

<script>
import Card from '@/components/elements/Card.vue'

export default {
  name: 'MainComponent',
  components: {
    Card
  },
  props: {
  },
  setup () {
    return {
    }
  }
}
</script>

<style lang="scss" scoped>
    .main {
        display: flex;
        padding-bottom: 295px;
        flex-direction: column;
        align-items: center;
        background: #FFF;
    }
    .books {
        display: flex;
        align-items: flex-start;
        justify-content: center;
        flex-wrap: wrap;
        gap: 26px;
        margin-top: 235px;
    }
</style>
