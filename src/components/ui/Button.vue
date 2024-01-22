<template>
  <button class="button" type="submit">{{ caption }}</button>
</template>

<script>
export default {
  name: 'ButtonComponent',
  components: {
  },
  props: {
    caption: {
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
    .button {
        display: inline-flex;
        padding: 6px 38px;
        justify-content: center;
        align-items: center;
        gap: 10px;
        border-radius: 7px;
        background: #3278FF;
        color:#FFF;
        text-align: center;
        font-feature-settings: 'calt' off;
        font-family: 'Roboto';
        font-size: 20px;
        font-style: normal;
        font-weight: 500;
        line-height: 22px;
        letter-spacing: -0.4px;
        cursor: pointer;
    }
</style>
