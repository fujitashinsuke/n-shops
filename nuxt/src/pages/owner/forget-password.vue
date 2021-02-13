<template>
  <div class="reset" >
    <v-card class="text-center pa-1">
      <v-card-title class="justify-center display-1 mb-2">パスワードをリッセットする</v-card-title>
      <v-card-subtitle>
        登録したメールアドレスを入力し送信ボタンを押して下さい。
        <br>
        入力したメールアドレスに新パスワード登録のURLが届きます。
      </v-card-subtitle>

      <!-- reset form -->
      <v-card-text>
        <v-form ref="form" v-model="isFormValid" lazy-validation @submit.prevent="submit">
          <v-text-field
            v-model="email"
            :rules="[rules.required]"
            :validate-on-blur="false"
            :error="error"
            :error-messages="errorMessages"
            :label="$t('forgot.email')"
            name="email"
            outlined
            @keyup.enter="submit"
            @change="resetErrors"
            prepend-inner-icon="mdi-email"
          ></v-text-field>

          <v-btn
            :loading="isLoading"
            block
            x-large
            color="primary"
            @click="submit"
          >送信する</v-btn>
        </v-form>
      </v-card-text>
    </v-card>
  </div>
</template>

<script>
/*
|---------------------------------------------------------------------
| Forgot Page Component
|---------------------------------------------------------------------
|
| Template to send email to remember/replace password
|
*/
export default {
  layout: 'ownerloguin',
  data() {
    return {
      // reset button
      isLoading: false,

      // form
      isFormValid: true,
      email: '',

      // form error
      error: false,
      errorMessages: '',

      // input rules
      rules: {
        required: (value) => (value && Boolean(value)) || '必ず入力してください'
      }
    }
  },
  methods: {
    submit(e) {
      if (this.$refs.form.validate()) {
        console.log('submit')
      }
    },
    resetEmail(email, password) {
    },
    resetErrors() {
      this.error = false
      this.errorMessages = ''
    }
  }
}
</script>

<style>
.reset{
  width: 600px;
}
</style>
