<template>
  <div class="hello">
    <h1>{{ name }}</h1>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue, Watch, Emit } from "vue-property-decorator";

@Component
export default class Test extends Vue {
  @Prop({ default: "" }) msg: string | undefined;
  public get name() {
    return "123412-----" + this.msg;
  }
  // name: 'HelloWorld',
  // props: {
  //   msg: String,
  // },
}
</script>

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
