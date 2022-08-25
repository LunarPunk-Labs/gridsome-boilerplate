<template>
  <LayoutHero>
    <template slot="hero">
      <hero-container :bg="heroBG">
        <div class="text-center">
          <div> 
            <g-image
              src="@/assets/img/logo.png"
              width="130"
              height="65"
              alt="logo"
              fit="outside"
            /> 
          </div>
          <div>
            <!--- <h3> Systemic solutions</h3> --->
          </div>
        </div>
      </hero-container>
    </template>

    <div class="bg-white shadow-lg p-10">
      <p>
        <h1>
          Process Design Agency
        </h1>
      </p>
      <p>
        We help web3 refi projects in moving away from uncertainty towards scientifically verifiable outcomes.
        <!---
        We lead, serve and support creative initiatives by designing
        transformation pathways that move projects from their initial
        uncertainty towards determinate regenerative outcomes.
        -->
      </p>
      <div class="flex flex-wrap my-10">
        <card v-for="card in cards" v-bind="card" :key="card.title"></card>
      </div>

      <!--
        <p>
        In our view distributed Identity will:
        <ul class="list-disc py-4 px-4">
          <li> Bring trust back to the internet and become ubiquitous</li>
          <li> Merge with all things physical (Rivers, Forests, Cars, Devices)</li>
          <li> Create new forms of wealth via personal and local currencies</li>
          <li> Create new business models and decimate vendor lock-in by enabling data portability</li>
          <li> Positivly impact user experience through human centric design</li>
          <li> Enable a sense of agency and autonomy by requiring user consent</li>
          <li> Foster the bottom up and build flatter institutions</li>
          <li><strong> Build a resilient world </strong></li>
        </ul>
      </p> 
-->
    </div>
  </LayoutHero>
</template>

<script>
import Page from "../templates/Page.vue";
export default {
  metaInfo: {
    title: "Home",
  },
  data() {
    return {
      heroBG: "CosmicGeometry.png",
      cards: [
        {
          title: "People",
          img: "Cards/Three.png",
          content:
            "Generating collective capacity by shaping, holding and convening spaces.",
          link: "../enviromental",
        },
        {
          title: "Projects",
          img: "Cards/Six.png",
          content:
            "Methodology development and value chain weaving for refi and web3.",
          link: "../governance",
        },
        {
          title: "Process",
          img: "Cards/RoughNine.png",
          content:
            "Regenerative terraforming through transparent MRV protocols.",
          link: "../social",
        },
      ],
    };
  },
  components: { Page },
};
</script>
