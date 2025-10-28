<template>
    <div class="sm:w-[1000px] mx-auto shadow-lg rounded-xl p-4 flex grid grid-cols-1 sm:grid-cols-3">
      <div class="col-span-1">
        <div class="h-100 sm:flex justify-center shadow-md rounded-xl border-2 border-gray-300"> 
            <Dimkuai />
        </div>
        <div class="w-full h-78 mt-4 sm:flex justify-center shadow-md rounded-xl border-2 border-gray-300">
            <home />
        </div>
      </div>
      <div class="col-span-1 sm:col-span-2">
        <div class="sm:flex shadow-md rounded-xl border-2 border-gray-300  sm:ml-4 ">
          <textmk />
        </div>
      </div>
  </div>
</template>


<script> 
import Dimkuai from './dimkuai.vue';
import home from './home.vue';
import textmk from './textmk.vue';

export default {
  components: {
    Dimkuai,
    home,
    textmk
  },
  data() {
    return {
      message: 'Hello Vue!'
    }
  },
  methods: {
    sayHello() {
      alert(this.message)
    }
  }
}
</script>

<style>

</style>