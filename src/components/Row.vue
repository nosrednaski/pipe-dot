<template>
  <tr>
    <template v-for="(char, i) in chopString">
      <td :key="i">{{ char }}</td>
    </template>
  </tr>
</template>

<script>
export default {
  
  props: ['string'],
  
  computed: {
        chopString: function() {
            return this.string.split("");
        }
    }
  
}

</script>

<style scoped>
tr {
  height: 12.5%
}
td {
  width: 12.5%;
  position: relative;
  font-weight:bolder;
  font-size: 3rem;
}
</style>
