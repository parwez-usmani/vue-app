<template>
  <v-layout column>
     <v-flex xs12 class="text-xs-center" mt-5>
      <h3>Sign Up</h3>
    </v-flex>
    <v-flex xs12 sm6 offset-sm3 mt-3>
            <form class="user-modal-container" action="/" method="post">
            <div class="user-modal form-register">
              <div class="error-message" v-text="registerError"></div>
            <div class="input_bg">
            <label>*Account</label>
            <input type="text" name="account_id" placeholder="*Account ID" v-model="account_id" required="required">
            </div>
            <div class="input_bg">
            <label>*Password</label>
            <input type="password" name="password" placeholder="*Password" required="required">
             </div>
             <div class="input_bg">
            <label>*Name</label>
            <input type="text" name="name" placeholder="*Name" v-model="Name" required="required">
              </div>
              <div class="input_bg">
            <label>*Company</label>
            <input type="text" name="company" placeholder="*Company Name" v-model="company_name" required="required">
              </div>
              <div class="input_bg">
            <label>*Country</label>
            <select name="country">
            <option value="">Select country</option> 
            <option value="India">India</option>
            <option value="USA">USA</option>
            <option value="Austrlia">Austrlia</option>
            <option value="China">China</option>
            </select> 
          </div>
          <div class="input_bg">
            <label>*Time Zone</label>
            <select name="timezone">
            <option value="">Select Time Zone</option> 
            <option value="UTC +5:30 hours">UTC +5:30 hours</option>
            <option value="UTC +6:30 hours">UTC +6:30 hours</option>
            <option value="UTC +7:30 hours">UTC +7:30 hours</option>
            <option value="UTC +8:30 hours">UTC +8:30 hours</option>
            </select>
          </div>
          <div class="input_bg">
            <label>*Email</label> 
             <input type="email" name="email" placeholder="*Email" required="required">
           </div>
            </div>
            <div class="btn_bg_singup">
                <div class="check_bg">
                <input type="checkbox" name="checkbox" value="value"/>
                <label>I agree following terms and Condition.<span>Agreement</span> 
                </label>
              </div>
              <input type="submit" value="Register">
             <router-link to="/signin" class="login_btn">Login</router-link>
               </div>
              <div class="links">
              </div>
      </form>
    </v-flex>
  </v-layout>
</template>

<script>
export default {}
</script>

