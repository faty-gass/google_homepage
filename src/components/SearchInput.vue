<template>
  <div class="q-mx-sm">
    <q-input rounded outlined style="min-width: 30em" v-model="text">
      <template v-slot:prepend>
        <q-icon name="search" />
      </template>
      <template v-slot:append>
        <q-icon name="mic" @click="text = ''" class="cursor-pointer" />
      </template>
    </q-input>
    <div class="text-center q-my-lg q-gutter-x-md">
      <q-btn
        color="grey-2"
        text-color="black"
        text-weight-light
        label="Recherche Google"
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

<style></style>
