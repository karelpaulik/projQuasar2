<template>
  <q-layout view="hhh lpr lfr">
    <q-header elevated class="bg-primary text-white" height-hint="98">
      <q-toolbar align="center">
        <q-btn dense flat round icon="menu" @click="toggleLeftDrawer" />
        <q-toolbar-title>
          <q-avatar>
            <img src="https://cdn.quasar.dev/logo-v2/svg/logo-mono-white.svg">
          </q-avatar>
          Title
        </q-toolbar-title>
      </q-toolbar>
      <q-tabs align="center" no-caps="">
        <q-route-tab to="/" label="Page One" />
        <q-route-tab to="/images" label="Page Two"  />
        <q-route-tab to="/contacts" label="Page Three" />
      </q-tabs>
    </q-header>
    
    <q-drawer v-model="leftDrawerOpen" side="left" bordered :width="200" :breakpoint="500" persistent class="bg-grey-3">
      <!-- drawer content -->
      <q-list bordered separator>
        <q-item clickable v-ripple><NuxtLink to="/">Home page</NuxtLink></q-item>
        <q-item clickable><NuxtLink to="/images">Images</NuxtLink></q-item>
        <q-item v-ripple><NuxtLink to="/contacts">Contacts</NuxtLink></q-item>
        <q-item><q-icon name="phone_iphone" />Item</q-item>
      </q-list>
      <div><q-icon name="phone_iphone" size="30px" color="teal"/>Item1</div>
      <div><q-icon name="o_phone_iphone" size="30px" color="teal"/>Item2</div>

      <div><q-icon name="phone_android" size="30px" color="teal"/></div>
      <div><q-icon name="o_phone_android" size="30px" color="teal"/></div>

      <div><q-icon name="keyboard" size="30px" color="teal"/></div>
      <div><q-icon name="o_keyboard" size="30px" color="teal"/></div>

      <div><q-icon name="connected_tv" size="30px" color="teal"/></div>
      <div><q-icon name="o_connected_tv" size="30px" color="teal"/></div>

      <div><q-icon name="thumb_up" size="md" color="pink-3" /></div>
      <div><q-icon name="o_thumb_up" size="md" color="teal-14" /></div>

    </q-drawer>

    <q-page-container>
      <q-page class="bg-teal-2">
        <NuxtPage />
        <!-- <router-view /> -->
      </q-page>
    </q-page-container>
  </q-layout>
</template>

<script setup>
import { ref } from 'vue'

import { useQuasar } from 'quasar'
const $q = useQuasar()

console.log($q.iconSet);

const leftDrawerOpen = ref(false)

function toggleLeftDrawer () {
  leftDrawerOpen.value = !leftDrawerOpen.value
}

</script>