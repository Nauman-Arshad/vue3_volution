
<template>
  <!-- <h5>Hello {{name}}</h5>
  <div v-html="channel"></div>
  <h2 v-bind:id="headingId">Heading</h2>
  <h2 class="underline">Underline text</h2>
  <h3 v-bind:class="status">Status</h3>
  <h2 v-bind:class="isPromoted && 'promoted'">Promoted Movie</h2>
  <h2 v-bind:class="isSoldout ? 'sold_out' : 'new'">Sold out movie</h2> -->
  <!-- <h2 v-if="num === 0">The number is zero</h2>
  <h2 v-else-if="num < 0">The number is Negative</h2>
  <h2 v-else-if="num > 0">The number is Positive</h2>
  <h2 v-else>Not a Number</h2>
<div v-if="display">
  <h2>Hello</h2>
  <h2>Nauman</h2>
  <h2>Vue</h2>
  </div> -->
  <!-- <template>
  <h2 v-if="num === 0">Number is 0</h2>
  <h2 v-else-if="num > 0">Number is +</h2>
  <h2 v-else-if="num < 0">Number is -</h2>
  <h2 v-else>Not a Number</h2>
  </template>
  <h2 v-show="showElement">using v-show</h2> -->
  <!-- <h5 v-for="name in names" :key="name">{{name}}</h5>
  <h5 v-for="name in fullnames" :key="name.first">{{name.first}} {{name.last}}</h5> -->
<form>
  <div>
    <label for="name">Name</label>
    <input type="text" id="name" v-model="formValues.name">
  </div>
</form>

</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      // name: 'Nauman',
      // channel: '<b>codecode</b>',
      // headingId: 'heading',
      // isPromoted: true,
      // isSoldout: true
      // num: 12,
      // display: true
      // showElement: true
      // names: ['Nauman', 'Nan', 'ken', 'Nap'],
      // fullnames: [
      //   { first: 'Nan', last: 'War' },
      //   {first: 'Loop', last: 'J'},
      //   { first: 'Man', last: 'Jes' }
      // ]
      formValues: {
        name: ''
      }
    };
  }
}
</script>

<style>
.underline{
  text-decoration: underline;
}
.promoted{
  font-style: italic;
}

.new{
  color: green;
}
.sold_out{
  color: orange
}
</style>
