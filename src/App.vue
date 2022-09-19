<template>
<div>
  <h5>Hello {{name}}</h5>
  <div v-html="channel"></div>
  <h2 :id="headingId">Heading</h2>
  <h2 class="underline">Underline text</h2>
  <h3 :class="status">Status</h3>
  <h2 :class="isPromoted && 'promoted'">Promoted Movie</h2>
  <h2 :class="isSoldout ? 'sold_out' : 'new'">Sold out movie</h2>
</div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      name: 'Nauman',
      channel: '<b>codecode</b>',
      headingId: 'heading',
      isPromoted: true,
      isSoldout: true
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
