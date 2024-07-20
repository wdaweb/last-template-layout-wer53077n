<template>
  <v-app>
    <v-app-bar color="#FF9800" prominent>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title>LOGO</v-toolbar-title>

      <v-spacer></v-spacer>

      <template v-if="$vuetify.display.mdAndUp">
        <v-btn prepend-icon="mdi-magnify" variant="text"></v-btn>
        <v-btn prepend-icon="mdi-filter" variant="text"></v-btn>
      </template>

      <v-btn prepend-icon="mdi-dots-vertical" variant="text"></v-btn>
    </v-app-bar>

    <v-navigation-drawer
      v-model="drawer"
      :location="$vuetify.display.mobile ? 'bottom' : undefined"
      temporary
    >
      <v-list>
        <v-list-item v-for="item in items" :key="item.title" @click="">
          <v-list-item-title>{{ item.title }}</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-main>
      <!----------------------------- 輪播圖 --------------------------->
      <carousel></carousel>
      <!---------------------------- 卡片組合 ----------------------------->
      <sectionOne class="section1"></sectionOne>
      <!---------------------------- 大圖壓字 ----------------------------->
      <sectionTwo class="section2"></sectionTwo>
    </v-main>

    <!---------------------------- Footer ----------------------------->
    <Footer />
  </v-app>
</template>

<script setup>
import carousel from "@/components/carousel.vue";
import sectionOne from "@/components/sectionOne.vue";
import sectionTwo from "@/components/sectionTwo.vue";
import Footer from "@/components/footer.vue";
</script>

<!-- NAVBAR的JS -->
<script>
export default {
  data: () => ({
    drawer: false,
    items: [
      { title: "HOME" },
      { title: "STORE" },
      { title: "ABOUT" },
      { title: "CONTACT" },
    ],
  }),

  watch: {
    group() {
      this.drawer = false;
    },
  },
};
</script>

<style scoped lang="scss">
.section1 {
  width: 100vw;
}
.section2 {
  display: flex;
}
</style>
