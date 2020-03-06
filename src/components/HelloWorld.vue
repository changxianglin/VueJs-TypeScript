<template>
  <div class="hello">
    <h1>{{msg}}</h1>
    <h1>{{test}}</h1>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      test: "Hello TS!" as string
    }
  },
  methods: {
    pressMe(): string {
      return this.test + 'banana'
    }
  }
})
</script>

// import { Component, Prop, Vue } from 'vue-property-decorator';

// @Component
// export default class HelloWorld extends Vue {
//   @Prop() private msg!: string;
//   firstName = "Hello World!"
//   lastName = 'Hello Wrold'
//   counter = 0

//   mounted() {
//     console.log('mounted')
//   }

//   get fullName(): string {
//     return this.firstName + this.lastName
//   }

//   IncrementCounter() {
//     this.counter++
//   }

// }
// </script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
