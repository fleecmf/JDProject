<template>
  <section :class="[panelClasss,cname]">
    <h4>-{{title}}-</h4>
    <slot></slot>
  </section>
</template>

<script>
export default {
  name: "panel",
  props: {
    cname: {
      default: "",
      tyoe: String
    },
    title: {
      default: "",
      tyoe: String
    }
  },
  data() {
    return {
      panelClasss: "panel"
    };
  },
  components: {}
};
</script>

<style lang="scss">
  @import "../../css/element.scss";

  .panel {
    @include panel;
  }
</style>
