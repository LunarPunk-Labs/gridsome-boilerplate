<template>
  <LayoutSplash>
    <template slot="hero">
      <hero-container :bg="heroBG">
        <div class="text-center">
          <div> 
            <g-image
              src="@/assets/img/logo.png"
              width="350"
              height="250"
              alt="logo"
              fit="outside"
              class="mb-10"
            /> 
          </div>
          <div>
            <!--- <h3> Systemic solutions</h3> --->
          </div>
        </div>
      </hero-container>
    </template>
  </LayoutSplash>
</template>

<script>
import Page from "../templates/Page.vue";
export default {
  data() {
    return {
      heroBG: "CosmicGeometry.jpg",
    };
  },
  components: { Page },
};
</script>
