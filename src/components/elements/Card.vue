<template>
  <div class="card">
    <img :src="preview" alt="image" class="card__image">
    <div class="card__info">
        <p class="card__name">{{name}}</p>
        <p class="card__autor">{{autor}}</p>
    </div>
    <Button class="card__button"
        caption="Купить"
    />
  </div>
</template>

<script>
import Button from '@/components/ui/Button.vue'
export default {
  name: 'CardComponent',
  components: {
    Button
  },
  props: {
    name: {
      type: String,
      default: ''
    },
    autor: {
      type: String,
      default: ''
    },
    preview: {
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
    .card {
        width: 330px;
        border-radius: 10px;
        background: #FFF;
        box-shadow: 1px 1px 4px 0px rgba(0, 0, 0, 0.30);
        padding: 19px 0px 24px 0px;
        display: flex;
        flex-direction: column;
        align-items: center;
        color:#000;
        font-family: 'Roboto';
        font-size: 20px;
        font-style: normal;
        font-weight: 400;
        line-height: normal;

        &__info {
            display: inline-flex;
            flex-direction: column;
            align-items: center;
            gap: 14px;
            width: 295px;
            height: 93px;
            margin-top: 14px;
        }

        &__name {
            margin: 0;
            font-size: 24px;
            text-align: center;
        }

        &__autor {
            margin: 0;
        }

        &__button {
            margin-top: 34px;
        }

    }
</style>
