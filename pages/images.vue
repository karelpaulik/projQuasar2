<template>
    <div class="row wrap justify-center items-start q-pa-md q-gutter-md">
        <q-card class="my-card bg-teal-1" style="width: 500px;">
            <!-- <img src="https://cdn.quasar.dev/img/mountains.jpg"> -->
            <q-img src="https://cdn.quasar.dev/img/mountains.jpg" >
                <div class="absolute-bottom text-subtitle1 text-center">
                    Caption
                </div>
            </q-img>

            <q-card-section>
                <q-btn color="white" text-color="black" label="Standard" @click="msg"/>
                <div class="text-h6">Our Changing Planet</div>
                <div class="text-subtitle2">by John Doe</div>
            </q-card-section>
            
            <q-card-section class="q-pt-none bg-white">
                Text
                <!-- <q-btn color="white" text-color="black" label="Standard" /> -->
            </q-card-section>
        </q-card>

        <q-card class="my-card bg-teal-1" style="width: 500px;">
            <img src="https://cdn.quasar.dev/img/mountains.jpg">

            <q-card-section>
                <div class="text-h6">Our Changing Planet</div>
                <div class="text-subtitle2">by John Doe</div>
            </q-card-section>

            <q-card-section class="q-pt-none">
                Text
            </q-card-section>
        </q-card>

        <q-card class="my-card bg-teal-1" style="width: 500px;">
            <img src="https://cdn.quasar.dev/img/mountains.jpg">

            <q-card-section>
                <q-btn color="white" text-color="black" label="Standard" @click="msg"/>
                <div class="text-h6">Our Changing Planet</div>
                <div class="text-subtitle2">by John Doe</div>
            </q-card-section>

            <q-card-section class="q-pt-none">
                Text
                <q-btn color="white" text-color="black" label="Standard" />
            </q-card-section>
        </q-card>

        <q-card class="my-card bg-teal-1" style="width: 500px;">
            <img src="https://cdn.quasar.dev/img/mountains.jpg">

            <q-card-section>
                <div class="text-h6">Our Changing Planet</div>
                <div class="text-subtitle2">by John Doe</div>
            </q-card-section>

            <q-card-section class="q-pt-none">
                Text
            </q-card-section>
        </q-card>

        <q-card class="my-card bg-teal-1" style="width: 500px;">
            <img src="https://cdn.quasar.dev/img/mountains.jpg">

            <q-card-section>
                <q-btn color="white" text-color="black" label="Standard" @click="msg"/>
                <div class="text-h6">Our Changing Planet</div>
                <div class="text-subtitle2">by John Doe</div>
            </q-card-section>

            <q-card-section class="q-pt-none">
                Text
                <q-btn color="white" text-color="black" label="Standard" />
            </q-card-section>
        </q-card>

        <q-card class="my-card bg-teal-1" style="width: 500px;">
            <img src="https://cdn.quasar.dev/img/mountains.jpg">

            <q-card-section>
                <div class="text-h6">Our Changing Planet</div>
                <div class="text-subtitle2">by John Doe</div>
            </q-card-section>

            <q-card-section class="q-pt-none">
                Text
            </q-card-section>
        </q-card>


    </div>
</template>

<script setup>

function msg() {
    alert("asdf");
}
</script>