<template>
  <div class="h-screen overflow-hidden">
    <g-image
      v-if="bg"
      :src="setImage"
      class="w-full h-screen object-cover absolute z-10 top-0 hero-image opacity-80"
      alt="cell"
    />
    <div
      class="relative z-10 h-screen px-4 flex justify-center items-center text-white"
    >
      <slot />
    </div>
  </div>
</template>
<style lang="scss" scoped>
.hero-image {
  // mix-blend-mode: luminosity;
}
</style>

<script>
export default {
  props: {
    bg: {
      required: false,
    },
  },
  computed: {
    setImage: function() {
      return require("@/assets/img/" + this.bg);
    },
  },
};
</script>
