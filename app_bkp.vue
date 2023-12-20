<template>
  <div>
    <h1>Nadpis</h1>
    <p>Odstavec textu normálního</p>
    <div class="q-pa-md bg-red-2">
      <div class="text-h1">Nadpis quasar textu</div>
      <p class="text-body1">Odstavec textu quasar</p>
      <p class="text-body2">Odstavec textu quasar</p>
    </div>
    Odstavec textu bez tagu p.
    <br>
    <br>
    <br>

    <div class="row bg-teal">
      <div class="col q-ma-md bg-teal-2">asdf</div>
      <div class="col q-ma-md bg-teal-2">asdf</div>
      <div class="col q-ma-md bg-teal-2">asdf</div>
    </div>

    <br>
    <div :class="row1">
      <div :class="itm1">asdf</div>
      <div :class="itm1">asdf</div>
      <div :class="itm1">asdf</div>
    </div>

  </div>
</template>

<script setup>
import { ref, reactive } from 'vue'

const row1 = "row bg-blue"
const itm1 = "col q-ma-md bg-blue-2 text-black"

</script>


<style>
</style>