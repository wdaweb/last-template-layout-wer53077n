<template>
  <v-container>
    <v-row>
      <v-col cols="12" class="text-center">
        <div class="topTitle">
          <h1>Bakery Items</h1>
          <h3>
            Duis aute irure dolor in reprehenderit in voluptate velit esse
            cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat
            cupidatat non proident, sunt in culpa qui officia deserunt.
          </h3>
        </div>
      </v-col>
    </v-row>
    <div data-aos="fade-up">
      <v-row sm="12" md="12" lg="3">
        <v-col>
          <v-card
            class="mx-auto text-center"
            style="background: #fff"
            max-width="344"
          >
            <v-img
              height="200px"
              src="https://picsum.photos/500/400?random=1"
              cover
            ></v-img>

            <v-card-title style="color: black"> BAGUETTE </v-card-title>

            <v-card-subtitle style="color: black">
              Small-batch sourdough baguette.
            </v-card-subtitle>
            <v-card-text style="color: #bf360c; font-size: 25px"
              >$4.5</v-card-text
            >
          </v-card>
        </v-col>
        <v-col>
          <v-card
            class="mx-auto text-center"
            style="background: #fff"
            max-width="344"
          >
            <v-img
              height="200px"
              src="https://picsum.photos/500/400?random=2"
              cover
            ></v-img>

            <v-card-title style="color: black"> FARMING BREAD </v-card-title>

            <v-card-subtitle style="color: black">
              Sample text. Click to select the Text Element.
            </v-card-subtitle>
            <v-card-text style="color: #bf360c; font-size: 25px"
              >$4.5</v-card-text
            >
          </v-card>
        </v-col>
        <v-col>
          <v-card
            class="mx-auto text-center"
            style="background: #fff"
            max-width="344"
          >
            <v-img
              height="200px"
              src="https://picsum.photos/500/400?random=3"
              cover
            ></v-img>

            <v-card-title style="color: black"> MIXED GRAIN </v-card-title>

            <v-card-subtitle style="color: black">
              Sample text. Click to select the Text Element.
            </v-card-subtitle>
            <v-card-text style="color: #bf360c; font-size: 25px"
              >$3.5</v-card-text
            >
          </v-card>
        </v-col>
        <v-col>
          <v-card
            class="mx-auto text-center"
            style="background: #fff"
            max-width="344"
          >
            <v-img
              height="200px"
              src="https://picsum.photos/500/400?random=4"
              cover
            ></v-img>

            <v-card-title style="color: black"> MILK BREAD </v-card-title>

            <v-card-subtitle style="color: black">
              Sample text. Click to select the Text Element.
            </v-card-subtitle>
            <v-card-text style="color: #bf360c; font-size: 25px"
              >$2.25</v-card-text
            >
          </v-card>
        </v-col>
        <v-col>
          <v-card
            class="mx-auto text-center"
            style="background: #fff"
            max-width="344"
          >
            <v-img
              height="200px"
              src="https://picsum.photos/500/400?random=5"
              cover
            ></v-img>

            <v-card-title style="color: black"> CHEESE BREAD </v-card-title>

            <v-card-subtitle style="color: black">
              Sample text. Click to select the Text Element.
            </v-card-subtitle>
            <v-card-text style="color: #bf360c; font-size: 25px"
              >$5.5</v-card-text
            >
          </v-card>
        </v-col>
        <v-col>
          <v-card
            class="mx-auto text-center"
            style="background: #fff"
            max-width="344"
          >
            <v-img
              height="200px"
              src="https://picsum.photos/500/400?random=6"
              cover
            ></v-img>

            <v-card-title style="color: black"> BAGUETTE </v-card-title>

            <v-card-subtitle style="color: black">
              Small-batch sourdough baguette.
            </v-card-subtitle>
            <v-card-text style="color: #bf360c; font-size: 25px"
              >$4.5</v-card-text
            >
          </v-card>
        </v-col>
      </v-row>
    </div>
  </v-container>
</template>

<script>
import AOS from "aos";
import "aos/dist/aos.css";

export default {
  mounted() {
    AOS.init();
  },
  data: () => ({
    show: false,
  }),
};
</script>

<style scoped lang="scss">
@import "aos/dist/aos.css";

.topTitle {
  text-align: center;
  margin: 2rem;
  padding: 5rem;
}
.v-container {
  margin-bottom: 5rem;
}
</style>
