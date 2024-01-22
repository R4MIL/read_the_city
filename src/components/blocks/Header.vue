<template>
  <header class="header">
    <img class="header__logo" src="@/components/icons/Logo.svg" alt="logo">
    <p class="header__phone">{{ phone }}</p>
  </header>
</template>

<script>
export default {
  name: 'HeaderComponent',
  props: {
    phone: {
      type: String,
      default: ''
    }
  },
  setup () {
    return {
    }
  }
}
</script>

<style lang="scss" scoped>
    .header {
        display: flex;
        height: 60px;
        padding: 13px 70px;
        justify-content: space-between;
        align-items: center;
        background: #3278FF;
        height: 34px;

        &__phone {
            font-family: 'Roboto';
            font-size: 22px;
            font-style: normal;
            font-weight: 700;
            line-height: normal;
            color: #FFF;
        }
    }
</style>
