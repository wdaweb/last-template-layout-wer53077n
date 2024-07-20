<template>
  <v-row>
    <v-col cols="12" class="image-container">
      <img class="bigImage" src="https://picsum.photos/1280/600/?random=10" />
      <div class="text-overlay">
        <div data-aos="zoom-in">
          <h1>Roll, proof, and bake. Every day.</h1>
          <p>
            When it comes to bread and sandwiches, freshness equals quality.
            That's why we bake our loaves, bagels, and sweet treats every single
            morning for maximum freshness.
          </p>
        </div>
        <v-row justify="center" style="margin: 1.5rem">
          <v-col cols="auto">
            <v-btn height="50" color="#FF9800" style="border-radius: 50px">
              SEE FUll Meun
            </v-btn>
          </v-col>
          <v-col cols="auto">
            <v-btn :ripple="false" height="50" style="border-radius: 50px">
              Order Now
            </v-btn>
          </v-col>
        </v-row>
      </div>
    </v-col>
  </v-row>
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
.image-container {
  position: relative;
  width: 100%;
  height: 600px;
}

.bigImage {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.text-overlay {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: white;
  text-align: center;
  padding: 20px;
}

.text-overlay h1 {
  margin: 0;
  font-size: 2.5rem;
}

.text-overlay p {
  margin: 10px 0 0;
  font-size: 1.25rem;
}
@media (max-width: 600px) {
  .image-container {
    height: 400px;
  }

  .text-overlay h1 {
    margin-top: 10rem;
    font-size: 1.5rem;
  }

  .text-overlay p {
    font-size: 1rem;
  }

  .text-overlay v-btn {
    height: 10px;
  }
}
</style>
