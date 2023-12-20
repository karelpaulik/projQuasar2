<template>
    <div class="text-h3">Index page</div>
    <div>
    <q-icon :name="matMenu" size="md" color="teal"/>
    <q-icon :name="fasFont" />
    <q-btn :icon="mdiAbTesting" />
    <p>Odstavec textu</p>
  </div>
</template>

<script setup>
import { matMenu } from '@quasar/extras/material-icons'
import { mdiAbTesting } from '@quasar/extras/mdi-v6'
import { fasFont } from '@quasar/extras/fontawesome-v5'
</script>