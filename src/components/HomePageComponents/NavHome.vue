<template>
  <nav class="cairo-font bg-[#98C1D9] py-12 px-25 flex items-center justify-start">
    <div class="text-white text-4xl font-bold ml-20">صوت</div>
    <ul class="flex space-x-40 text-white text-lg pl-20">
      <li><RouterLink to="/register" class="hover:underline">تسجيل الدخول</RouterLink></li>
      <li><RouterLink to="/" class="hover:underline">التسجيل</RouterLink></li>
      <li><RouterLink to="/" class="hover:underline">اتصل بنا</RouterLink></li>
      <li>
        <button @click="toggleDropdown" class="hover:underline">عن الموقع</button>
        <ul v-if="isDropdownOpen" class="bg-white text-black absolute p-4 shadow-lg rounded-md">
          <li><a href="#">معلومات</a></li>
          <li><a href="#">المزيد</a></li>
        </ul>
      </li>
    </ul>
  </nav>
</template>

<script>
import { RouterLink } from 'vue-router'

export default {
  name: 'NavComponent',
  data() {
    return {
      isDropdownOpen: false,
    }
  },
  methods: {
    toggleDropdown() {
      this.isDropdownOpen = !this.isDropdownOpen // Toggle dropdown
    },
  },
}
</script>
