<template>
  <div class="v">
    <h1>BMI CALCULATOR</h1>
    <label for="">weight:kg</label><br />
    <input v-model="weight" type="number" placeholder="null" /><br />
    <label for="">height:m</label><br />
    <input v-model="height" type="number" placeholder="null" /><br />
    <!-- <button  v-if="result" onclick="result">result</button><br /> -->
    <!-- <p v-if="result">{{ result }}</p> -->
    <p>the BMI is{{ result }}</p>
  </div>
</template>
 <script>
export default {
  data() {
    return {
      height: null,
      weight: null,
    };
  },
  // method: {
  //   divide() {
  //     return this.weight / this.height;
  //   },
  // },
  computed: {
    result() {
      return this.weight / (this.height * this.height);
    },
  },
};
</script>jixara1969@acuxi.com
<style>
label {
  color: rgb(220, 101, 101);
  justify-content: center;
  text-align: center;
  align-items: center;
}
input {
  color: brown;
  background-color: aquamarine;
  justify-content: center;
  align-items: center;
  text-align: center;
  border-radius: 30px;
}
button {
  color: brown;
  background-color: bisque;
}
.v {
  justify-content: center;
  align-items: center;
  background-color: khaki;
}
* {
  max-width: 250px;
  border-radius: 6px;
}
h1 {
  font-size: 20px;
}
</style>
