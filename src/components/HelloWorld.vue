<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "HelloWorld",
  data() {
    return {
      msg: "Hello TypeScript" as string | number
    };
  },
  // computed: {
  //   getLength(): string {
  //     return this.msg;
  //   },
  // },
  methods:{
    changeMsg(msg:string | number){
      return this.msg = msg
    }
  }
});
</script>
