<template lang="html">
  <button :class="[btnClass, cname]">
    <slot></slot>
  </button>
  
</template>

<script>
export default {
  props: {
    cname: {
      default: "",
      tyoe: String
    }
  },
  data() {
    return {
      btnClass: 'btn',

    }
  }
}
</script>

<style lang="scss">
  @import "../../css/element.scss";

  .btn {
    @include btn;
  }
</style>
