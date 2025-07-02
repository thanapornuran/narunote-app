<!-- layouts/default.vue -->
<template>
  <div class="flex h-screen bg-[#271c19]">
    <!-- Sidebar -->
    <aside class="w-64 bg-[#55423d] shadow-[0_2px_8px_0_#140d0b]">
      <div class="flex flex-col h-full">
        <!-- Logo/Brand -->
        <div class="flex items-center justify-center h-16 px-4 border-b border-[#140d0b]">
          <img src="/favicon.ico" alt="" class="w-6 h-6 mr-2" />
          <h1 class="text-xl font-bold text-[#fffffe]">
            Narunote
          </h1>
        </div>

        <!-- Navigation Menu -->
        <nav class="flex-1 px-4 py-6 space-y-2">
          <p class="text-[#fff3ec] font-bold my-3">
            <UIcon name="mingcute:home-2-fill" class="w-5 h-5 mr-2 inline-block" />
            Diary & Mood
          </p>

          <NuxtLink to="/diary/mood" class="flex items-center px-4 py-2 rounded-lg transition-colors duration-200" :class="[
            route.path === '/diary/mood' 
            ? 'text-[#e78fb3] bg-[#271c19] border-r-2 border-[#e78fb3]' 
            : 'text-[#fff3ec]'
          ]">
            <UIcon name="mingcute:emoji-2-fill" class="w-5 h-5 mr-3"
              :class="route.path === '/diary/mood' ? 'text-[#e78fb3]' : 'text-[#fff3ec]'" />
            <span class="">Mood</span>
          </NuxtLink>

          <NuxtLink to="/diary/sleep" class="flex items-center px-4 py-2 rounded-lg transition-colors duration-200" :class="[
            route.path === '/diary/sleep' 
            ? 'text-[#e78fb3] bg-[#271c19] border-r-2 border-[#e78fb3]' 
            : 'text-[#fff3ec]'
          ]">
            <UIcon name="mingcute:moon-line" class="w-5 h-5 mr-3"
              :class="route.path === '/diary/sleep' ? 'text-[#e78fb3]' : 'text-[#fff3ec]'" />
            <span class="">Sleep</span>
          </NuxtLink>

          <NuxtLink to="/diary/journal" class="flex items-center px-4 py-2 rounded-lg transition-colors duration-200" :class="[
            route.path === '/diary/journal' 
            ? 'text-[#e78fb3] bg-[#271c19] border-r-2 border-[#e78fb3]' 
            : 'text-[#fff3ec]'
          ]">
            <UIcon name="mingcute:book-2-line" class="w-5 h-5 mr-3"
              :class="route.path === '/diary/journal' ? 'text-[#e78fb3]' : 'text-[#fff3ec]'" />
            <span class="">Diary</span>
          </NuxtLink>

          <hr class="my-4 border-[#3d2c28]" />

          <p class="text-[#fff3ec] font-bold my-3">
            <UIcon name="mingcute:bling-fill" class="w-5 h-5 mr-2 inline-block" />
            Calendar
          </p>

          <NuxtLink to="/calendar" class="flex items-center px-4 py-2 rounded-lg transition-colors duration-200" :class="[
            route.path === '/calendar' 
            ? 'text-[#e78fb3] bg-[#271c19] border-r-2 border-[#e78fb3]' 
            : 'text-[#fff3ec]'
          ]">
            <UIcon name="mingcute:calendar-2-line" class="w-5 h-5 mr-3"
              :class="route.path === '/calendar' ? 'text-[#e78fb3]' : 'text-[#fff3ec]'" />
            <span class="">Calendar</span>
          </NuxtLink>

          <hr class="my-4 border-[#3d2c28]" />

          <p class="text-[#fff3ec] font-bold my-3">
            <UIcon name="mingcute:bling-fill" class="w-5 h-5 mr-2 inline-block" />
            Wishlist
          </p>

          <NuxtLink to="/wishlist/beauty" class="flex items-center px-4 py-2 rounded-lg transition-colors duration-200" :class="[
            route.path.startsWith('/wishlist/beauty') 
            ? 'text-[#e78fb3] bg-[#271c19] border-r-2 border-[#e78fb3]' 
            : 'text-[#fff3ec]'
          ]">
            <UIcon name="mingcute:lipstick-line" class="w-5 h-5 mr-3"
              :class="route.path.startsWith('/wishlist/beauty') ? 'text-[#e78fb3]' : 'text-[#fff3ec]'" />
            <span class="">Beauty</span>
          </NuxtLink>

          <NuxtLink to="/wishlist/food" class="flex items-center px-4 py-2 rounded-lg transition-colors duration-200" :class="[
            route.path.startsWith('/wishlist/food') 
            ? 'text-[#e78fb3] bg-[#271c19] border-r-2 border-[#e78fb3]' 
            : 'text-[#fff3ec]'
          ]">
            <UIcon name="mingcute:birthday-2-fill" class="w-5 h-5 mr-3"
              :class="route.path.startsWith('/wishlist/food') ? 'text-[#e78fb3]' : 'text-[#fff3ec]'" />
            <span class="">Food</span>
          </NuxtLink>

          <NuxtLink to="/wishlist/general" class="flex items-center px-4 py-2 rounded-lg transition-colors duration-200" :class="[
            route.path.startsWith('/wishlist/general') 
            ? 'text-[#e78fb3] bg-[#271c19] border-r-2 border-[#e78fb3]' 
            : 'text-[#fff3ec]'
          ]">
            <UIcon name="mingcute:gift-line" class="w-5 h-5 mr-3"
              :class="route.path.startsWith('/wishlist/general') ? 'text-[#e78fb3]' : 'text-[#fff3ec]'" />
            <span class="">General</span>
          </NuxtLink>

          <hr class="my-4 border-[#3d2c28]" />

          <p class="text-[#fff3ec] font-bold my-3">
            <UIcon name="mingcute:bling-fill" class="w-5 h-5 mr-2 inline-block" />
            Expenses
          </p>

          <NuxtLink to="/expenses" class="flex items-center px-4 py-2 rounded-lg transition-colors duration-200" :class="[
            route.path === '/expenses' 
            ? 'text-[#e78fb3] bg-[#271c19] border-r-2 border-[#e78fb3]' 
            : 'text-[#fff3ec]'
          ]">
            <UIcon name="mingcute:wallet-4-fill" class="w-5 h-5 mr-3"
              :class="route.path === '/expenses' ? 'text-[#e78fb3]' : 'text-[#fff3ec]'" />
            <span class="">Expenses</span>
          </NuxtLink>
        </nav>

        <!-- User Section (Optional) -->
        <div class="px-4 py-4 border-t border-[#140d0b]">
          <div class="flex items-center">
            <UAvatar src="https://avatars.githubusercontent.com/u/739984?v=4" alt="User Avatar" size="sm" />
            <div class="ml-3">
              <p class="text-sm  text-[#fffffe]">
                John Doe
              </p>
              <p class="text-xs text-[#fff3ec]">
                john@example.com
              </p>
            </div>
          </div>
        </div>
      </div>
    </aside>
  </div>
</template>

<script setup>
  import {
    computed
  } from 'vue'
  import '@/assets/css/main.css'

  const colorMode = useColorMode()
  const route = useRoute()

  const isDark = computed(() => colorMode.value === 'dark')

  const toggleColorMode = () => {
    colorMode.preference = colorMode.value === 'dark' ? 'light' : 'dark'
  }

  const getPageTitle = () => {
    const routeMap = {
      '/': 'Home',
      '/dashboard': 'Dashboard'
    }
    return routeMap[route.path] || 'Page'
  }

  const toggleSidebar = () => {
    // Mobile sidebar toggle logic can be added here
    console.log('Toggle sidebar for mobile')
  }
</script>

<style scoped>
  /* Additional custom styles if needed */
  /* .router-link-active {
  @apply bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300;
} */
</style>