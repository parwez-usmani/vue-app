<template>
  <v-layout column>
     <v-flex xs12 class="text-xs-center" mt-5>
      <h3>Sign In</h3>
    </v-flex>
    <v-flex xs12 sm6 offset-sm3 mt-3>
            <form class="user-modal-container" action="/" method="post">
            <div class="user-modal form-register">
              <div class="error-message" v-text="registerError"></div>
              <div class="input_bg">
              <label>*Account ID</label>
              <input type="text" name="account_id" placeholder="Account ID" v-model="account_id" required="required">
            </div>
            <div class="input_bg">
               <label>*Password</label>
               <input type="password" name="password" placeholder="Password" required="required">
               </div>
            </div>
             <div class="btn_bg_singup signin">
              <input type="submit" value="Login">
              <div class="link_singin">
               <router-link to="/Resetpassword">Forget Password</router-link>
                <router-link to="/resend_verification_email">Resend Verification Email</router-link>
               <router-link to="/signup">Sign Up</router-link>
              </div>
              </div>              
      </form>
    </v-flex>
  </v-layout>
</template>

<script>
export default {}
</script>
