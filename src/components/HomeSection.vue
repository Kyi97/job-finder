<template>
  <div style="position: relative">
    <v-img
      src="../assets/yellowspot.png"
      style="position: absolute; z-index: 1"
    />
    <v-row>
      <v-flex
        xs12
        md6
        class="text-center"
        style="position: relative; z-index: 2"
      >
        <p>
          <span style="font-size: 35px; font-weight: bolder"
            >Find Your Dream</span
          ><br />
          <span style="color: #f59d1e; font-size: 50px; font-weight: bolder"
            >Job And
          </span>
          <br />
          <span style="color: #f59d1e; font-size: 50px; font-weight: bolder"
            >Career <span style="color: black">To </span></span
          ><br />
          <span style="color: black; font-size: 50px; font-weight: bolder"
            >Build a Life</span
          >
        </p>
      </v-flex>

      <v-flex
        xs12
        md6
        class="text-center"
        style="position: relative; z-index: 2"
      >
        <img src="../assets/main.png" alt="An image" class="responsive-img" />
      </v-flex>
      <v-img
        src="../assets/bluespot.png"
        style="position: absolute; z-index: 1; right: 0"
      />
      <v-img
        src="../assets/bluespot.png"
        style="position: absolute; z-index: 1; right: 0; left: 0"
        width="50"
      />
      <img
        src="../assets/purplespot.png"
        style="
          position: absolute;
          z-index: 1;
          top: 50%;
          left: 50%;
          transform: translate(-50%, -50%);
        "
        width="80"
      />
      <img
        src="../assets/yellowspot.png"
        style="
          position: absolute;
          z-index: 1;
          top: 60%;
          left: 60%;
          transform: translate(-50%, -50%);
        "
        width="80"
      />
    </v-row>
  </div>
</template>
<script>
export default {
  name: "HomeSection",
  data: () => ({}),
};
</script>