<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
      </div>

      <v-spacer></v-spacer>
      <v-btn text to="/" tag="router-link">地域選択</v-btn>
      <v-btn text to="/forecast" tag="router-link">天気予報</v-btn>
      <v-btn text to="/caution" tag="router-link">注意報</v-btn> <!-- 購入ビューを追加 -->
      <v-btn text to="/purchase" tag="router-link">参照API</v-btn>
      <v-btn
        href="https://www.jma.go.jp/bosai/forecast/"
        target="_blank"
        text
      >
        <span class="mr-2">Forecast Resource</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>
