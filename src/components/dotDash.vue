<template>
  <div class="hello">
          {{ chopPipe }}
<hr>
    <table>
      <tr>
        <td>x</td>
        <td>o</td>
        <td>o</td>
        <td>-</td>
        <td>|</td>
      </tr>
      <tr>
        <td>|</td>
        <td>o</td>
        <td>-</td>
        <td>-</td>
        <td>|</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  name: 'dotDash',
  data() {
    return {
      pipeString: "xo-|-||oo|xxo--||-ox-ooxxo|o|----|xo-|x|xoxxo|x-|-||-ooxoox-|x-o",
    }
  },
  computed: {
    chopPipe: function() {
      let arr = this.pipeString.split('')
      let h1s = arr.forEach((x) => {{ x }})
      return h1s;
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  table {
    border: solid 1px
  }
</style>
