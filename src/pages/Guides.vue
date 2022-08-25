<template>
  <LayoutHero>
    <div class="bg-white shadow-lg p-10">
      <h2>Guides</h2>
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
