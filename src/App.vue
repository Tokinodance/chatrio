<template>
	<div class="login-container">
	    <div class="login-box">
	      <h2 class="title">Login</h2>
	      <form class="form">
	        <div class="form-group">
	         <label for="username" class="label">邮箱:</label>
	          <input type="text" id="username" v-model="username" class="input" />
	        </div>

	        <div class="form-group">
	          <label for="password" class="label">密码:</label>
	          <input type="password" id="password" v-model="password" class="input" />
	        </div>

	        <button type="button" @click="login" class="button">登录</button>
	      </form>
	  </div>
  </div>
</template>

<style scoped>
  .login-container {

    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: rgb(42, 98, 133);
    background-image: linear-gradient(#e66465, #9198e5);
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.3);
  }

  .login-box {
    width: 500px;
    padding: 30px;
    background-color: rgba(233, 183, 239, 0.79);
    background-image: linear-gradient(#a6dbf6, #fa4f4f);

    border-radius: 5px;
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
  }

  .title {
    margin-bottom: 30px;
  }

  .form {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background-color: rgba(225, 238, 217, 0.74);
    //background-image: linear-gradient(#679db9, #e87474);

    padding: 30px;
    border-radius: 5px;
  }

  .form-group {
    margin-bottom: 30px;
    width: 100%;
  }

  .label {
    display: block;
    margin-bottom: 5px;
    font-size: 16px;
    font-weight: bold;
  }

  .input {
    display: block;
    width: 100%;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
    font-size: 16px;
  }

  .button {
    padding: 10px;
    background-color: #007bff;
    color: #fff;
    border: none;
    border-radius: 5px;
    font-size: 16px;
    cursor: pointer;
  }

  .button:hover {
    background-color: #0069d9;
  }
</style>
