<template>
  <div>
    <Headerx />
    <q-page class="flex column flex-center ">
      <img
        class="q-mb-lg"
        alt="Quasar logo"
        src="~assets/Google_2015_logo.svg"
      />
      <SearchInput />
      <p>
        Google disponible en :
        <a
          id="lang-link"
          href="https://www.google.fr/setprefs?sig=0_0ss7ucIRZcuFnhnJmzXrc2giHlA%3D&hl=en&source=homepage&sa=X&ved=0ahUKEwi01MzYyb_uAhWSz4UKHW8vA6QQ2ZgBCA8"
          >English</a
        >
      </p>
    </q-page>
    <Footerx />
  </div>
</template>

<script>
import SearchInput from "src/components/SearchInput.vue";
import Headerx from "src/components/Headerx.vue";
import Footerx from "src/components/Footerx.vue";
export default {
  components: { SearchInput, Headerx, Footerx },
  name: "PageIndex"
};
</script>
<style>
a {
  text-decoration: none !important;
  color: black !important;
}
a:hover {
  text-decoration: underline !important;
}
#lang-link {
  color: blue !important;
}
</style>
