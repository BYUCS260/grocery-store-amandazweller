<template>
  <div>
    <CartList :cart="cart" />
  </div>
</template>

<script>
import CartList from "../components/CartList.vue"
export default {
  name: 'Cart-List',
  components: {
    CartList
  },
  computed: {
    cart() {
      return this.$root.$data.cart;
    }
  },

}
</script>
