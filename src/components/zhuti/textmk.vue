<template>
  <div class=" w-full p-2 h-screen overflow-y-auto">
    <div v-for="(item, index) in source" :key="index" class="p-4  hover:bg-cyan-50 cursor-pointer transition-transform duration-300 transform hover:scale-102 shadow-lg rounded-lg">
      <div class="text-lg font-bold text-cyan-400 border-b-2 border-cyan-200">
        <h1>{{ item.title }}</h1>
      </div>
      <div class="mt-2 text-sm font-bold text-pink-300">
        <p>时间：{{ item.time }}</p>
      </div>
      <div class="mt-2 text-sm font-bold">
        <h2>{{ item.content }}</h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      source: [
        {
          title: "制作移动端点击按钮",
          time: "2025年11月3日",
          content: "制作移动端点击按钮，页面优化Ciallo～(∠・ω< )⌒★,最近制作缓慢，这个网站差不多是个人练习的项目，JavaScript，HTML，CSS，Tailwindcss，Vue，Netlify，Astro，还有很多技术要学习，慢慢来(๑・̀ㅂ・́)و✧"
        },
        {
          title: "小小的页面优化",
          time: "2025年10月28日",
          content: "我重构标签页面与日记，解决了部分内容超出部分的方式，下次开发移动端按钮展开跳转(๑・̀ㅂ・́)و✧"
        },
        {
          title: "astro静态开发,版本10.0发布",
          time: "2025年10月22日",
          content: "关于astro静态开发的最新版本发布，欢迎大家使用！因为是第一次制作，这个还叫不上网站的网页,还有很多不完善的地方，后续会慢慢完善的。目前只有一个页面，就制作了pc端的页面和移动端的页面，使用移动端的页面还没有做完，所以按钮还没有做(⁄ ⁄・⁄ω⁄・⁄ ⁄)"
        },
        {
          title: "网站制作使用Astro",
          time: "2025年10月15日",
          content: "我在制作网站时，使用了Astro，vue,tailwindcss，netlify等技术，在制作中学习tailwindcss的使用方法，git的使用方法，netlify的使用方法，Astro的使用方法等等。简单来说5天速成3天模拟，自己制作练练手。Ciallo～(∠・ω< )⌒★"
        },
        {
          title: "我的第一个想法",
          time: "2025年10月13日",
          content: "我发现了一个很酷的网站，netlify，可以免费部署自己的静态网站，而且可以绑定自己的域名，真是太方便了！嘻嘻主要免费！！！冲鸭～ (๑・̀ㅂ・́)و✧"
        },
      ]
    }
  }
}
</script>

<style>

</style>

<style scoped>

</style>

