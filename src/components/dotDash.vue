
<template>
  <div>
    <table>
      <template v-for="(string, i) in chopPipe" :index="i">
        <Row :key="i" :string="string"></Row>
      </template>
    </table>
  </div>
</template>

<script>
import Row from './Row.vue'

export default {

  name: 'dotDash',
  components: { Row },  
  data() {
    return {
      pipeString: "xo-|-||oo|xxo--||-ox-ooxxo|o|----|xo-|x|xoxxo|x-|-||-ooxoox-|x-o",
    }
  },
  computed: {
    chopPipe: function() {
      // let arr = this.pipeString.split('')
      // let h1s = arr.forEach((x) => {{ x }})
      // return h1s;
      let arr = this.pipeString.match(/.{1,8}/g);
      // let arr2 = arr.split("");
      return arr
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
table {
  width: 480px;
  height: 480px;
  border: solid black 1px
}

/* td {
  width: 33.33%;
  position: relative;
  font-weight: bold;
} */
/* td:after {
  content: '';
  display: block;
  margin-top: 100%;
}
td .content {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  background: gold;
} */
</style>
