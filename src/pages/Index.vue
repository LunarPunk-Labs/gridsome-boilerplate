<template>
  <LayoutHero>
    <template slot="hero">
      <hero-container :bg="heroBG">
        <div  class="text-center">
          <div>
              <g-image
            src="@/assets/img/logo.png"
            width="300"
            height="150"
            alt="logo"
            fit="outside"
          />
          </div>
          <div>
            <h3> Systemic solutions</h3>
          </div>
        </div>
      </hero-container>
    </template>

    <div class="flex flex-wrap my-10">
      <card v-for="card in cards" v-bind="card" :key="card.title"></card>
    </div>

    <div class="bg-white shadow-lg p-10">
      <h2>Our thesis</h2>
      <p>
        According to <a href="https://carbontracker.org/reports/2020-vision-why-you-should-see-the-fossil-fuel-peak-coming/">CarbonTracker.org</a>, the fossil fuel industry is looking at $25tn of fixed assets vunerable to stranding with systemic risks to financial markets as they seek to divest. 
        Fund managers are resultently looking to balance their risk through ESG investments (Enviromental, Social, Governance). 
        The true value of these organisations will very likely be unlocked and accelerated by "Self Soverign Identity" and "Web of Trust" technology. 
      </p>

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
    </div>
  </LayoutHero>
</template>

<script>
export default {
  metaInfo: {
    title: "Home",
  },
  data() {
    return {
      heroBG: "bg.jpg",
      cards: [
        {
          title: "Enviromental",
          // img: "enviromentalmoon.jpg",
          content:
            "We design and build biomimetic technology intended to drive the restoration and regeneration of our biosphere from a living systems perspective",
          link: "../enviromental",
        },
        {
          title: "Social",
          // img: "socialbonfiremoon2.jpg",
          content:
            "We're a distributed organisation made from an ecology of peers that come and go. A structured network of solidarity and mutual care",
          link: "../social",
        },
        {
          title: "Governace",
          // img: "gonvernancemoon.jpg",
          content:
            "We're transparent about our activities and are collectivly governed by the internal and external stakeholders involved with our network",
          link: "../governance",
        },
      ],
    };
  },
};
</script>