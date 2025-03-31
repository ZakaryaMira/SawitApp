<template>
  <nav class="bg-[#98C1D9] grid grid-cols-3 items-center h-25 p-5">
    <!-- right -->
    <div class="text-white text-4xl font-bold text-right">صوت</div>
    <!-- middel -->
    <div></div>

    <!-- left -->
    <div class="flex items-centre justify-end text-white text-lg gap-5">
      <img :src="NotificationLogo" class="w-9 h-9" />
      <span>اسم المسير</span>
      <img :src="UserLogo" class="w-9 h-9" />
    </div>
  </nav>
</template>
<script>
import NotificationLogo from '@/SVG/NotificationLogo.svg'
import UserLogo from '@/SVG/UserLogo.svg'
export default {
  data() {
    return {
      NotificationLogo,
      UserLogo,
    }
  },
}
</script>
