<template>
  <div class="register-page">
    <div class="form">
      <div class="login">
        <div class="login-header">
          <h3>REGISTER</h3>
          <p>Please register if you are a new member</p>
        </div>
      </div>
      <form class="login-form">
        <input type="text" placeholder="username" />
        <input type="email" placeholder="email" />
        <input type="number" placeholder="contact" />
        <input type="password" placeholder="password" />
        <button @click="navigateToFund">Register</button>
      </form>
    </div>
  </div>
</template>
<script>
export default {
  name: 'Register',
    methods: {
      navigateToRegister() {
            this.$router.push('/register');
      },
      navigateToFund() {
      this.$router.push('/fund');
      }
    }
}
</script>


<style>
@import url(https://fonts.googleapis.com/css?family=Roboto:300);

header .header {
  background-color: #fff;
  height: 45px;
}


.register-page {
  width: 360px;
  padding: 4% 0 0;
  margin: auto;
}

.register-page .form .login {
  margin-top: -31px;
  margin-bottom: 26px;
}

.form {
  position: relative;
  z-index: 1;
  background: #FFFFFF;
  max-width: 360px;
  margin: 0 auto 100px;
  padding: 45px;
  text-align: center;
  box-shadow: 0 0 20px 0 rgba(0, 0, 0, 0.2), 0 5px 5px 0 rgba(0, 0, 0, 0.24);
}

.form input {
  font-family: "Roboto", sans-serif;
  outline: 0;
  background: #f2f2f2;
  width: 100%;
  border: 0;
  margin: 0 0 15px;
  padding: 15px;
  box-sizing: border-box;
  font-size: 14px;
}

.form button {
  font-family: "Roboto", sans-serif;
  text-transform: uppercase;
  outline: 0;
  background-color: #328f8a;
  background-image: linear-gradient(45deg, #328f8a, #08ac4b);
  width: 100%;
  border: 0;
  padding: 15px;
  color: #FFFFFF;
  font-size: 14px;
  -webkit-transition: all 0.3 ease;
  transition: all 0.3 ease;
  cursor: pointer;
}

.form .message {
  margin: 15px 0 0;
  color: #b3b3b3;
  font-size: 12px;
}

.form .message a {
  color: #4CAF50;
  text-decoration: none;
}

body {
  background-color: #328f8a;
   background-image: url('@/assets/kid.png');
   height: 100vh;
   background-position: center;
   background-repeat: no-repeat;
  font-family: "Roboto", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>