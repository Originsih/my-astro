<template>
  <nav>
    <div class="sm:w-[1000px] mx-auto shadow-md rounded-xl h-16 bg-white">
        <div class="justify-between items-center h-16 px-4 grid grid-cols-1 w-full sm:grid-cols-3">
            <div class="sm:block col-span-1 sm:col-span-1 ">
              <div class="flex items-center justify-between">
                <div class="hidden sm:flex items-center ">
                  <img src="/images/30.png" alt="示例图片" class="w-12 h-12 rounded-xl shadow-md mr-4"/>
                  <h1 class="sm:text-gray-800 font-bold text-lg text-shadow-md">{{ Survivor }}</h1>
                </div>
                  <Button/>
              </div>

          </div>
            <div class="hidden sm:block col-span-1 sm:col-span-1 ">
              <a href="/" class="text-gray-500 hover:text-pink-300 font-medium text-base sm:text-xl transition-colors mr-6">
                <i class="fa-solid fa-house"></i>
                {{ name }}
              </a>
              <a href="/blog" class="text-gray-500 hover:text-pink-300 font-medium text-base sm:text-xl transition-colors mr-6">
                <i class="fa-solid fa-phone"></i>
                {{ logo }}
              </a>
                <a href="/guanyu" class="text-gray-500 hover:text-pink-300 font-medium text-base sm:text-xl transition-colors mr-6">
                  <i class="fa-solid fa-info-circle mr-1"></i>
                  {{ about }}
                </a>
            </div>
            <div class="hidden sm:block col-span-1 sm:col-span-1">
              <!-- 搜索框 -->
              <div class="relative"> 
                <input type="text" class="w-full h-10 px-4 py-2 bg-gray-100 border border-gray-200 rounded-md focus:outline-none focus:border-pink-500" placeholder="搜索">
                <button type="submit" class="absolute right-0 top-0 mt-2 mr-2">
                  <i class="fa-solid fa-magnifying-glass"></i>
                </button>
              </div>
            </div>
        </div>
    </div>
  </nav>
</template>

<script>
import Button from './Button.vue';
export default {
  props: {
    name: {type: String, default: '首页'},
    logo: {type: String, default: '友联'},
    about: {type: String, default: '关于'},
    Survivor: {type: String, default: 'Survivor'},
  },
  components: {
    Button
  }
}
</script>

<style>
button {
  cursor: pointer;
  background: transparent;
  border: none;
  padding: 0;
}

a, button, i {
  transition: all 0.2s ease;
}
</style>