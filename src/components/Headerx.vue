<template>
  <div class="text-right q-ma-lg q-gutter-x-md">
    <a href="https://mail.google.com/mail/?tab=wm&ogbl">Gmail</a>
    <a href="https://www.google.fr/imghp?hl=fr&tab=wi&ogbl">Images</a>
    <q-icon name="apps" style="color:#6D676B; font-size: 2em" />
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
export default {};
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
}
</style>
