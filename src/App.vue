<template>
<div>
  <h5>Hello {{name}}</h5>
  <div v-html="channel"></div>
  <h2 v-bind:id="headingId">Heading</h2>
</div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      name: 'Nauman',
      channel: '<b>codecode</b>',
      headingId: 'heading'
    };
  }
}
</script>

<style>

</style>
