<template>
<div class="login-container">
  <h1>登入</h1>
  <form>
    <p ref="testp">test p</p>
      <nav>
    <router-link to="/ProductInfo">ProductInfo</router-link> |
    <router-link to="SalesRecordView">Sales Record</router-link>
  </nav>
  <router-view/>
    <input type="text" placeholder="帳號" required>
    <input type="password" placeholder="密碼" required>
    <button type="submit" @click="login">登入</button>
  </form>
</div>
  </template>
<script>
  export default {
    name: 'LoginView',
    methods: {
    login() {
      // 簡化範例：假設登入成功 
      this.$router.push('/about')
    //   if (this.username === 'admin' && this.password === '1234') {
    //     // 導向主頁
    //     this.$router.push('/')
    //   } else {
    //     alert('帳號或密碼錯誤')
    //   }
    }
    },
    mounted(){
        let m = this.$refs.testp.textContent;
        //let m = this.$ref.testp.textContent;
        alert(m);
    }
  }
  

</script>
<style>
body {
  background-image: url("https://images.unsplash.com/photo-1508701921662-c7c5714b9858?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTd8fGNvbXB1dGVyfGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=500&q=60");
  background-size: cover;
  font-family: sans-serif;
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  margin: 0;
}

.login-container {
  background-color: rgba(255, 255, 255, 0.8);
  padding: 20px;
  border-radius: 5px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

.login-container input[type="text"],
.login-container input[type="password"] {
  width: 100%;
  padding: 10px;
  margin-bottom: 10px;
  border: 1px solid #ccc;
  border-radius: 3px;
  box-sizing: border-box;
}

.login-container button {
  background-color: #4CAF50;
  color: white;
  padding: 10px 15px;
  border: none;
  border-radius: 3px;
  cursor: pointer;
}
</style>