<template>
  <div class="q-mx-sm text-center">
    <div id="searchbar">
      <q-input rounded outlined v-model="text" dense>
        <template v-slot:prepend>
          <q-icon name="search" />
        </template>
        <template v-slot:append>
          <q-icon name="mic" class="cursor-pointer" />
          <q-tooltip content-class="bg-black"
            >Utiliser la recherche vocale</q-tooltip
          >
        </template>
      </q-input>
    </div>
    <div class="text-center q-my-lg q-gutter-x-md">
      <q-btn
        color="grey-2"
        text-color="black"
        label="Recherche Google"
        @click="text = ''"
        no-caps
      />
      <q-btn
        color="grey-2"
        text-color="black"
        label="J'ai de la chance"
        no-caps
      />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: ""
    };
  }
};
</script>

<style scoped>
#searchbar {
  width: 50vw !important;
}

@media screen and (max-width: 850px) {
  #searchbar {
    width: 80vw !important;
  }
}
</style>
