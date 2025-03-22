<template>
  <section class="cairo-font bg-[#98C1D9] py-40 px-45 flex items-center justify-end">
    <div class="information-home">
      <h1 class="text-4xl font-bold mb-4 text-white">تصويت آمن عبر الإنترنت</h1>
      <p class="text-lg mb-6 text-white">
        قم بانشاء انتخابات لمدرستك او مؤسستك في ثوان , <br />
        يمكن للمصوتين التصويت من اي مكان على جهاز الحاسوب الخاص بهم
      </p>
      <button
        @click="changeText"
        class="bg-[#EE6C4D] text-white px-20 py-5 rounded-md text-lg font-semibold hover:bg-orange-600 transition"
      >
        {{ buttonText }}
      </button>
    </div>
    <div class="photo-home">
      <img :src="VotingHome" alt="" class="w-220 h-102" />
    </div>
  </section>
</template>

<script>
import VotingHome from '@/SVG/VotingHome.svg'
export default {
  name: 'Home',
  data() {
    return {
      VotingHome,
      buttonText: 'انشاء انتخابك الان',
    }
  },
  methods: {
    changeText() {
      this.buttonText = 'جاري التحميل'
    },
  },
}
</script>
