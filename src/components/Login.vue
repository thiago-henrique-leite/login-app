<template>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
  <div class="main">
    <div class="login">
      <form>
        <label>Log in</label>
        <p class="options">Log in with one of the following options.</p>
        <div class="social-container">  
          <div class="social"><i class="fa fab fa-google"></i></div>
          <div class="social"><i class="fa fab fa-apple"></i></div>
        </div>
        <p class="input-label">Email</p>
        <input type="email" name="email" placeholder="Enter your email" required=""/>
        <p class="input-label">Password</p>
        <input type="password" name="pswd" placeholder="Enter your password" required=""/>
        <button>Log in</button>
        <p class="signup">Dont have an account?<a href="#">Sign up</a></p>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      form: {
        email: "",
        password: ""
      }
    }
  },
 
  methods: {
    login() {},
    register() {},
  }
}
</script>

<style>
  body {
    marging: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    font-family: 'Jost', sans-serif;
    background: #F5F5F5;
  }

  a {
    color: #fff;
    text-decoration: none;
    margin: 0px 7px;
  }

  a:hover {
    color: #79d1ff;
  }

  p {
    color: #909090;
  }

  label {
    color: #fff;
    font-size: 2.3em;
    justify-content: left;
    display: flex;
    margin: 0px 30px;
    padding-top: 50px;
    font-weight: bold;
  }

  .main {
    width: 400px;
    height: 800px;
    background-color: #151515;
    border-radius: 50px;
    box-shadow: 5px 5px 40px #000;
  }

  .login {
    position: relative;
    width: 100%;
    height: 100%;
  }

  .options {
    margin: 30px auto;
    justify-content: left;
    display: flex;
    padding: 0px 8%;
  }

  .social-container {
    padding-left: 20px;
  }

  .social {
    margin: 0px 10px;
    background: #312c2c;
    border: 1px solid #4f4a4a;
    height: 55px;
    width: 41%;
    display: inline-flex;
    justify-content: center;
    align-items: center;
    border-radius: 10px;
    cursor: pointer;
    font-size: 26px;
    color: white;
  }

  .social:hover {
    background: #3498db;
  }

  p.input-label {
    padding-left: 30px;
    margin: 20px 0px;
    color: #dbdbdb;
  }

  input {
    width: 80%;
    height: 30px;
    background: #312c2c;
    justify-content: center;
    display: flex;
    margin: 0px auto;
    padding: 10px;
    border: 1px solid #4f4a4a;
    outline: none;
    border-radius: 10px;
    text-indent: 10px;
    color: #fff;
    font-size: 15px;
    letter-spacing: 0.09em;
  }

  input:focus { 
    border: solid 1px #d2afff;
  }

  button {
    width: 85%;
    height: 50px;
    margin: 10px auto;
    justify-content: center;
    display: block;
    color: #f5f5f5;
    background: linear-gradient(45deg, #d2afff, #c82f63);
    font-size: 1.2em;
    margin-top: 45px;
    outline: none;
    border: none;
    border-radius: 10px;
    cursor: pointer;
  }

  button:hover {
    background: #3498db;
  }

  .signup {
    margin: 30px auto;
    justify-content: center;
    display: flex;
    font-weight: bold;
  }
</style>
