<template>
  <v-app id="App" class="vh-100">
    <v-container fluid class="pa-0">
      <div class="row">
        <div class="col-12">
          <v-btn class="mx-auto my-1" large color="primary" @click="count++">Primary</v-btn>          
        </div>
        <div class="col-12">
          <!-- <v-btn class="mx-auto my-1" large color="primary" @click="count++">Primary</v-btn>           -->
          <div class="mx-auto border border-danger" style="max-width:300px">
            <h1>123</h1>
          </div>
        </div>
        <div class="col-12">
          <v-card
            class="mx-auto my-2"
            max-width="400"
            tile
            v-for="(item,idx) in ' '.repeat(count).split('')"
            :key="idx"
          >
            <v-list-item class>
              <v-list-item-content>
                <v-list-item-title>Single-line item</v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-card>
        </div>
      </div>
    </v-container>
  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld';

export default {
  name: "App",

  components: {
    // HelloWorld,
  },

  data: () => {
    return {
      items: [],
      count: 1
    };
  }
};
</script>

<style>
/* @import "../node_modules/bootstrap/dist/css/bootstrap.min.css" */
</style>;