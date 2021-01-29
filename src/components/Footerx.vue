<template>
  <q-footer id="footerx" class="q-pa-md">
    <p class="q-ml-md">France</p>
    <div class="q-gutter-md">
      <div class="flex row flex-wrap justify-around q-gutter-md ">
        <div>
          <img src="~assets/leaf.png" alt="leaf" style="width: 13px" />
          <a
            class="links q-mx-sm"
            href="https://sustainability.google/intl/fr/commitments-europe/?utm_source=googlehpfooter&utm_medium=housepromos&utm_campaign=bottom-footer&utm_content="
            >Neutre en carbonne depuis 2007</a
          >
        </div>
        <div class="q-gutter-md">
          <a
            v-for="(item, idx) in footerLinks1"
            :key="idx"
            :href="item.link"
            class="links text-no-wrap"
            >{{ item.content }}</a
          >
        </div>
      </div>
      <div class="flex row q-gutter-md ">
        <a
          v-for="(item, idx) in footerLinks2"
          :key="idx"
          :href="item.link"
          class="links text-no-wrap "
          >{{ item.content }}</a
        >
      </div>
    </div>
  </q-footer>
</template>

<script>
export default {
  data() {
    return {
      footerLinks1: [
        {
          content: "Info consommateurs",
          link:
            "https://support.google.com/websearch?p=fr_consumer_info&hl=fr&fg=1"
        },
        {
          content: "Confidentialité",
          link: "https://policies.google.com/privacy?hl=fr&fg=1"
        },
        {
          content: "Conditions",
          link: "https://policies.google.com/terms?hl=fr&fg=1"
        },
        {
          content: "Paramètres",
          link: "https://www.google.fr/preferences?hl=fr"
        }
      ],
      footerLinks2: [
        {
          content: "Publicité",
          link:
            "https://www.google.fr/intl/fr_fr/ads/?subid=ww-ww-et-g-awa-a-g_hpafoot1_1!o2&utm_source=google.com&utm_medium=referral&utm_campaign=google_hpafooter&fg=1"
        },
        {
          content: "Entreprise",
          link:
            "https://www.google.fr/services/?subid=ww-ww-et-g-awa-a-g_hpbfoot1_1!o2&utm_source=google.com&utm_medium=referral&utm_campaign=google_hpbfooter&fg=1"
        },
        {
          content: "A propos",
          link:
            "https://about.google/?utm_source=google-FR&utm_medium=referral&utm_campaign=hp-footer&fg=1"
        },
        {
          content: "Comment fonctionne la recherche Google ?",
          link: "https://google.com/search/howsearchworks/?fg=1"
        }
      ]
    };
  }
};
</script>

<style>
#footerx {
  background-color: #e5e5e5 !important;
  color: rgb(67, 67, 67) !important;
}
.links {
  text-decoration: none !important;
  color: rgb(82, 82, 82) !important;
}
.links :hover {
  text-decoration: underline !important;
}
</style>
