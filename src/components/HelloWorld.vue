<template>
  <div class="hello">
    <!-- <h1>{{ msg }}</h1> -->
    <h1 >{{ book.title }}/{{ book.author }}/{{ book.year }}</h1>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
interface Book{
  title: string;
  author: string;
  year: number;
}
export default defineComponent({
  name: "HelloWorld",
  data() {
    return {
      // msg: "Hello TypeScript" as string | number
      book: {
        title: 'Vue 3 Guide',
        author: 'Vue Team',
        year: 2020
      } as Book
    };
  },
  // computed: {
  //   getLength(): string {
  //     return this.msg;
  //   },
  // },
  methods:{
    // changeMsg(msg:string | number){
    //   return this.msg = msg
    // }
 
  }
});
</script>
