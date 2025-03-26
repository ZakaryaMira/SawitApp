<template>
  <FormComponentTemplate
    title="صوت"
    :fileds="registerFields"
    buttonText="انشاء حساب"
    @submite="handleRegister"
  />
</template>

<script>
import FormComponentTemplate from '@/components/FormComponent/FormComponentTemplate.vue'
export default {
  components: { FormComponentTemplate },
  data() {
    return {
      registerFields: [
        { label: 'اسم المستخدم', placeholder: 'اسم المستخدم', type: 'text', value: '' },
        { label: 'البريد الالكتروني', placeholder: 'البريد الالكتروني', type: 'email', value: '' },
        { label: 'كلمة المرور', placeholder: 'كلمة المرور', type: 'password', value: '' },
        {
          label: 'تاكيد كلمة المرور',
          placeholder: 'تاكيد كلمة المرور',
          type: 'password',
          value: '',
        },
      ],
    }
  },
  methods: {
    handleRegister(data) {
      console.log(data)
    },
  },
}
</script>
