<template>
  <q-footer id="footerx">
    <p class=" q-px-lg q-py-sm" id="country">France</p>

    <div class="flex row wrap justify-around q-gutter-md q-mb-sm ">
      <div class="q-mx-auto">
        <img src="~assets/leaf.png" alt="leaf" style="width: 1em" />
        <a
          class="links q-mx-sm"
          href="https://sustainability.google/intl/fr/commitments-europe/?utm_source=googlehpfooter&utm_medium=housepromos&utm_campaign=bottom-footer&utm_content="
          >Neutre en carbonne depuis 2007</a
        >
      </div>
      <div class="q-gutter-x-md q-mx-auto">
        <a
          v-for="(item, idx) in footerLinks1"
          :key="idx"
          :href="item.link"
          class="links text-no-wrap"
          >{{ item.content }}</a
        >
      </div>
      <div class="flex row q-gutter-x-md q-mx-auto ">
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
  font-size: 12px;
}
.links :hover {
  text-decoration: underline !important;
}
#country {
  width: 100%;
  border-top: solid rgb(213, 213, 213) 1px;
  border-bottom: solid rgb(213, 213, 213) 1px;
}
</style>
