<template>
  <div class="text-right q-ma-md q-gutter-x-md">
    <a href="https://mail.google.com/mail/?tab=wm&ogbl">Gmail</a>
    <a href="https://www.google.fr/imghp?hl=fr&tab=wi&ogbl">Images</a>
    <q-btn icon="apps" flat text-color="grey-8">
      <q-menu anchor="bottom right" self="top middle" max-height="400px">
        <div
          class="flex justify-between wrap q-pa-md q-gutter-y-sm"
          style="width: 320px"
        >
          <div
            class="apps text-center q-px-md cursor-pointer"
            v-for="(app, idx) in googlesApps"
            :key="idx"
          >
            <img
              :src="require('../assets/google_' + app + '.svg')"
              style="width:55px"
              :alt="app"
            />
            <p>{{ upperCase(app) }}</p>
          </div>
        </div>
      </q-menu>
    </q-btn>
    <q-btn
      color="primary"
      type="a"
      href="https://accounts.google.com/ServiceLogin?hl=fr&passive=true&continue=https://www.google.fr/&ec=GAZAAQ"
      no-caps
      class="logBtn"
      >Connexion</q-btn
    >
  </div>
</template>

<script>
export default {
  data() {
    return {
      googlesApps: [
        "maps",
        "gmail",
        "drive",
        "agenda",
        "meet",
        "one",
        "photos",
        "shopping",
        "search"
      ]
    };
  },
  methods: {
    upperCase(word) {
      return word.charAt(0).toUpperCase() + word.slice(1);
    }
  }
};
</script>

<style scoped>
a {
  text-decoration: none !important;
  color: black !important;
  font-size: 13px !important;
  letter-spacing: normal !important;
}
a:hover {
  text-decoration: underline !important;
}
.logBtn {
  color: white !important;
  font-weight: bold;
}
.apps:hover {
  background: rgba(206, 220, 255, 0.604);
  border: solid white 1px;
  border-radius: 10px;
}
</style>
