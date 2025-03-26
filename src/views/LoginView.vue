<template>
  <FormComponentTemplate
    title="صوت"
    :fileds="loginFields"
    buttonText="تسجيل الدخول"
    @submite="handleLogin"
  />
</template>

<script>
import FormComponentTemplate from '@/components/FormComponent/FormComponentTemplate.vue'
export default {
  components: { FormComponentTemplate },
  data() {
    return {
      loginFields: [
        {
          label: 'البريد الالكتروني',
          type: 'email',
          placeholder: 'البريد الالكتروني',
          value: '',
        },
        {
          label: 'كلمة المرور',
          type: 'password',
          placeholder: 'كلمة المرور',
          value: '',
        },
      ],
    }
  },
}
</script>
<style></style>
