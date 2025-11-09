<template>
  <div class="overflow-y-auto h-80">
    <div class="mt-4 text-lg text-shadow-md text-center">
      <h1 class="text-center text-3xl font-bold mt-3">标签</h1>
    </div>
    <div  class="flex flex-wrap justify-center mt-4 ">
      <div v-for="(item, index) in items" :key="index" class="border-2 border-gray-200 rounded-md mr-2 mb-2 ml-2 p-2  hover:text-white hover:bg-pink-300 ">
        <h1 class="">{{item.names}}</h1>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          names: 'java',
        },
        {
          names: 'python',
        },
        {
          names: 'javascript',
        },
        {
          names: 'html',
        },
        {
          names: 'css',
        },
        {
          names: 'vue',
        },
        {
          names: 'node',
        },
        {
          names: 'php',
        },
        {
          names: 'linux',
        },
        {
          names: 'git',
        },
        {
          names: 'vscode',
        },
        {
          names: 'jquery',
        },
        {
          names: 'bootstrap',
        }
      ]
    }
  }
}
</script>

<style>

</style>