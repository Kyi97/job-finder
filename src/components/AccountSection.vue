<template>
  <div class="adjust">
    <v-row class="pt-15">
      <v-img src="../assets/yellowspot.png" class="yellowimg" />
      <v-flex xs12 md6 class="text-center flexpos">
        <img src="../assets/postjob.png" alt="Post" class="responsive-img" />
      </v-flex>
      <v-flex xs12 md6 class="text-center flexpos">
        <p class="text text-left">
          Build your personal<br />
          account profile
        </p>
        <p class="text-left">
          Lorem Ipsum is simply dummy text of the printing and typesetting
          industry. Lorem Ipsum has been the industry's standard dummy text ever
          since the 1500s, when an unknown printer took a galley of type and
          scrambled it to make a type specimen book. It has survived not only
          five centuries, but also the leap into electronic typesetting,
          remaining essentially unchanged.
        </p>
        <div class="d-flex ml-auto">
          <v-btn color="black" class="white--text">Post Job</v-btn>
        </div>
      </v-flex>
    </v-row>
  </div>
</template>
  <script>
export default {
  name: "HomeSection",
  data: () => ({}),
};
</script>
<style scoped>
.adjust {
  position: relative;
  margin-left: 5rem;
  margin-right: 5rem;
}
.text {
  font-size: 30px;
  font-weight: 500;
}
.yellowimg {
  position: absolute;
  z-index: 1;
}
.flexpos {
  position: relative;
  z-index: 2;
}
</style>