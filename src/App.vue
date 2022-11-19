<script setup lang="ts">
import {defineAsyncComponent} from "vue"

const Navbar = defineAsyncComponent(()=>import("./components/Navbar.vue"))
const Sidebar = defineAsyncComponent(()=>import("./components/Sidebar.vue"))
const PostList = defineAsyncComponent(()=>import("./components/Postlist.vue"))

</script>

<template>
  
  <div class="h-full w-full bg-black">
    <Navbar />

    <div class="max-w-6xl flex space-x-9 mt-5 mx-auto">
      <Sidebar />
      <PostList />
    </div>
  </div>

</template>


