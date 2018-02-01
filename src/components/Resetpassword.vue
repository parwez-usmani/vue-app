<template>
  <v-layout column>
     <v-flex xs12 class="text-xs-center" mt-5>
      <h3>Reset Password</h3>
    </v-flex>
    <v-flex xs12 sm6 offset-sm3 mt-3>
            <form class="user-modal-container" action="/" method="post">
            <div class="user-modal form-register">
              <div class="error-message" v-text="registerError"></div>
              <div class="input_bg"> 
              <label>*Email</label>             
               <input type="email" name="email" placeholder="Email" required="required">
             </div>
            </div>
            <div class="btn_bg_singup signin">                
              <input type="submit" id="registerSubmit" value="Reset Password">
              <router-link to="/signin" class="login_btn">Log In</router-link>
               </div>
              <div class="links"> <router-link to="/signin">Already have an account?</router-link>
              </div>
      </form>
    </v-flex>
  </v-layout>
</template>

<script>
export default {}
</script>