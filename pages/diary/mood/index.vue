<template>
  <div class="">
    <div class="flex items-center gap-3 mb-4">
      <span class="flex items-center text-[#fff3ec]">
        <UIcon name="mingcute:home-2-fill" class="mr-1.5" />
        Diary & Mood
      </span>

      <UIcon name="mingcute:right-fill" class="w-5 h-5 inline-block" />

      <span class="flex items-center text-[#ffc0ad] font-bold">
        <UIcon name="mingcute:emoji-2-fill" class="mr-1.5" />
        Mood
      </span>
    </div>

    <div>
      <img src="/icons/moods/angry-face.png" alt="" class="w-20 h-20 mb-4" />
      <img src="/icons/moods/cry.png" alt="" class="w-20 h-20 mb-4" />
      <img src="/icons/moods/happy.png" alt="" class="w-20 h-20 mb-4" />
      <img src="/icons/moods/hug.png" alt="" class="w-20 h-20 mb-4" />
      <img src="/icons/moods/kiss.png" alt="" class="w-20 h-20 mb-4" />
      <img src="/icons/moods/nausea.png" alt="" class="w-20 h-20 mb-4" />
      <img src="/icons/moods/sleep.png" alt="" class="w-20 h-20 mb-4" />
      <img src="/icons/moods/wink.png" alt="" class="w-20 h-20 mb-4" />

      <!-- <form class="bg-[#fff3ec] rounded-lg p-6 shadow-md max-w-md mx-auto">
        <div class="mb-4">
          <label for="mood" class="block text-[#ff8ba7] font-semibold mb-2">
            How are you feeling today?
          </label>
          <select id="mood" class="w-full p-2 rounded border border-[#ffc0ad] focus:outline-none focus:ring-2 focus:ring-[#ff8ba7]">
            <option value="">Select mood</option>
            <option value="happy">😊 Happy</option>
            <option value="sad">😢 Sad</option>
            <option value="excited">🤩 Excited</option>
            <option value="tired">😴 Tired</option>
            <option value="angry">😠 Angry</option>
          </select>
        </div>
        <div class="mb-4">
          <label for="note" class="block text-[#ff8ba7] font-semibold mb-2">
            Add a note
          </label>
          <textarea id="note" rows="3" class="w-full p-2 rounded border border-[#ffc0ad] focus:outline-none focus:ring-2 focus:ring-[#ff8ba7]" placeholder="Write something cute..."></textarea>
        </div>
        <button type="submit" class="bg-[#ff8ba7] text-white font-bold py-2 px-4 rounded hover:bg-[#ffc0ad] transition">
          Save Mood
        </button>
      </form> -->
    </div>
  </div>
</template>

<script lang="ts" setup>

</script>

<style scoped>
@import url('./assets/css/main.css');

body {
  /* font-family: 'RobotoItalic', sans-serif;
  background-color: var(--background-color);
  width: 100%; */
  color: #fffffe;
}

</style>