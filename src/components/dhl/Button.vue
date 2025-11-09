<template>
  <div class="sm:hidden relative mt-2">
    <!-- 触发按钮（右浮动） -->
    <div class="sm:float-right">
      <button  @click="isExpanded = !isExpanded" 
        class="w-12 h-12 rounded-full bg-gray-200 hover:bg-gray-300 transition-colors flex items-center justify-center"
        aria-label="切换展开状态">
        <!-- 动态切换图标：展开时显示关闭图标-->
        <i :class="isExpanded 
            ? 'fa-solid fa-times text-gray-700' 
            : 'fa-solid fa-bars text-gray-700'">
        </i>
      </button>
    </div>

    <!-- 展开内容区域 -->
    <div class="mt-2 overflow-hidden transition-all duration-300 ease-in-out"
      :style="{ 
        maxHeight: isExpanded ? '500px' : '0',  // 控制高度实现展开/收起
        opacity: isExpanded ? 1 : 0             // 透明度过渡增强效果
      }">
      <div class="p-4 bg-white border rounded-lg shadow-sm">
        <!-- 这里放展开后的内容 -->
        <h3 class="font-medium text-gray-800">展开内容标题</h3>
            <div class="sm:block col-span-1 sm:col-span-1 ">
              <a href="/" class="text-gray-500 hover:text-pink-300 font-medium text-base sm:text-xl transition-colors mr-6">
                <i class="fa-solid fa-house"></i>
                首页
              </a>
              <a href="/blog" class="text-gray-500 hover:text-pink-300 font-medium text-base sm:text-xl transition-colors mr-6">
                <i class="fa-solid fa-phone"></i>
                友联
              </a>
                <a href="/guanyu" class="text-gray-500 hover:text-pink-300 font-medium text-base sm:text-xl transition-colors mr-6">
                  <i class="fa-solid fa-info-circle mr-1"></i>
                关于
                </a>
            </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

// 定义展开状态的响应式变量（默认收起）
const isExpanded = ref(false)

</script>

<style scoped>
/* 可选：调整展开内容的定位，避免被其他元素遮挡 */
.relative {
  position: relative;
  z-index: 10;
}
</style>