<template>
  <LayoutHero>

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
          <li> Merge with and aggrigate all things physical (Rivers, Forests, Bioregions, Cars, Devices)</li>
          <li> Create new forms of wealth via personal and local currencies</li>
          <li> Create new business models and decimate vendor lock-in by enabling data portability</li>
          <li> Positivly impact user experience through human centric design</li>
          <li> Enable a sense of agency and autonomy through the requirement of user consent</li>
          <li> Bring trust back to the internet and become ubiquitous</li>
          <li> Foster the bottom up and build flatter institutions</li>
          <li><strong> Build a resilient world </strong></li>
        </ul>
      </p>
    </div>

    <div class="flex flex-wrap my-10">
      <card v-for="card in cards" v-bind="card" :key="card.title"></card>
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
            "Intractiblie global issues will be solved by aggrigatiing solutions that remain embedded in their local bioregional context ",
          link: "../enviromental",
        },
        {
          title: "Social",
          // img: "socialbonfiremoon2.jpg",
          content:
            "We need to raise capacity amongst the dispossessed and marginalised. The long tail of society will be the ones that solve global issues, not the top down",
          link: "../social",
        },
        {
          title: "Governace",
          // img: "gonvernancemoon.jpg",
          content:
            "Governance refers to the process of evolving the rules and protocols through which we interact. It is a shared language ",
          link: "../governance",
        },
      ],
    };
  },
};
</script>