<template>
  <div class="container-fluid">
    <header>
      <div class="card-header">
        <button></button>
        <a href="#" class="icon"></a>
        <span class="col-6">Sistema</span>
      </div>
    </header>
    <div>
    </div>
    <br />
    <div class="container">
      <div class="card-flex">
        <div class="row">
          <div class="col-6">
            <div class="login-wrap">
              <div class="login-html">
                <input
                  id="tab-1"
                  type="radio"
                  name="tab"
                  class="sign-in"
                  checked
                /><label for="tab-1" class="tab">Sistema</label>
                <input
                  id="tab-2"
                  type="radio"
                  name="tab"
                  class="for-pwd"
                /><label for="tab-2" class="tab"></label>
                <div class="login-form">
                  <div class="sign-in-htm">
                    <div class="group">
                      <label for="user" class="label">Usuario</label>
                      <input id="user" type="text" class="input" />
                    </div>
                    <div class="group">
                      <label for="pass" class="label">Contraseña</label>
                      <input
                        id="pass"
                        type="password"
                        class="input"
                        data-type="password"
                      />
                    </div>
                    <div class="group">
                      <input type="submit" class="button" value="Entrar" />
                    </div>
                    <div class="hr"></div>
                  </div>
                  <div class="for-pwd-htm">
                    <div class="group">
                      <label for="user" class="label">Username or Email</label>
                      <input id="user" type="text" class="input" />
                    </div>
                    <div class="group">
                      <input
                        type="submit"
                        class="button"
                        value="Reset Password"
                      />
                    </div>
                    <div class="hr"></div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <footer>
      <span class="span2">Adsi Centro Agroturistico @2021</span>
    </footer>
    <div>
      <button><i class="fas fa-align-left"></i></button>
    </div>
    <link rel="stylesheet" href="css/all.min.css">
  </div>
</template>
<script>

export default {
  name: "login",
  props: {
    login: String,
  },
};
</script>
<style>
.ser {
  font-family: "icons";
  margin-right: 5px;
  margin-top: -2px;
  font-size: 35px;
}
footer {
  background-color: rgb(26, 26, 218);
  margin-top: 20px;
}
header {
  border: 1px 1px solid black;
  margin-top: 0px;
  color: white;
  background-color: blue;
}
span {
  margin-right: 90%;
}
.container {
  color: black;
  background-color: white;
  padding-right: 50%;
}
.card-flex {
  border: 2px 2px 2px solid black;
}
b-card-text {
  text-transform: uppercase;
  font-size: 24px;
  background-color: rgb(120, 120, 236);
  color: white;
}
.span2 {
  color: white;
  margin-right: 100%;
}
/* Este es código del Login d ela página principal*/
.login-wrap{
	width: 100%;
	margin:auto;
	max-width:510px;
	min-height:510px;
	position:relative;
	background:url(https://maxcdn.icons8.com/app/uploads/2016/03/material-1-1000x563.jpg) no-repeat center;
	background-size: cover;
	box-shadow:0 12px 15px 0 rgba(0,0,0,.24),0 17px 50px 0 rgba(0,0,0,.19);
}
.login-html{
	width:100%;
	height:100%;
	position:absolute;
	padding:90px 70px 50px 70px;
	background:rgba(0,0,0,0.5);
}
.login-html .sign-in-htm,
.login-html .for-pwd-htm{
	top:0;
	left:0;
	right:0;
	bottom:0;
	position:absolute;
	-webkit-transform:rotateY(180deg);
	transform:rotateY(180deg);
	-webkit-backface-visibility:hidden;
	backface-visibility:hidden;
	-webkit-transition:all .4s linear;
	transition:all .4s linear;
}
.login-html .sign-in,
.login-html .for-pwd,
.login-form .group .check{
	display:none;
}
.login-html .tab,
.login-form .group .label,
.login-form .group .button{
	text-transform:uppercase;
}
.login-html .tab{
	font-size:22px;
	margin-right:15px;
	padding-bottom:5px;
	margin:0 15px 10px 0;
	display:inline-block;
	border-bottom:2px solid transparent;
}
.login-html .sign-in:checked + .tab,
.login-html .for-pwd:checked + .tab{
	color:#fff;
	border-color:#1161ee;
}
.login-form{
	min-height:345px;
	position:relative;
	-webkit-perspective:1000px;
	perspective:1000px;
	-webkit-transform-style:preserve-3d;
	transform-style:preserve-3d;
}
.login-form .group{
	margin-bottom:15px;
}
.login-form .group .label,
.login-form .group .input,
.login-form .group .button{
	width:100%;
	color:#fff;
	display:block;
}
.login-form .group .input,
.login-form .group .button{
	border:none;
	padding:15px 20px;
	border-radius:25px;
	background:rgba(255,255,255,.1);
}
.login-form .group input[data-type="password"]{
	-webkit-text-security:circle;
}
.login-form .group .label{
	color:#aaa;
	font-size:12px;
}
.login-form .group .button{
	background:#1161ee;
}
.login-form .group label .icon{
	width:15px;
	height:15px;
	border-radius:2px;
	position:relative;
	display:inline-block;
	background:rgba(255,255,255,.1);
}
.login-form .group label .icon:before,
.login-form .group label .icon:after{
	content:'';
	width:10px;
	height:2px;
	background:#fff;
	position:absolute;
	-webkit-transition:all .2s ease-in-out 0s;
	transition:all .2s ease-in-out 0s;
}
.login-form .group label .icon:before{
	left:3px;
	width:5px;
	bottom:6px;
	-webkit-transform:scale(0) rotate(0);
	transform:scale(0) rotate(0);
}
.login-form .group .check:checked + label{
	color:#fff;
}
.login-form .group .check:checked + label .icon{
	background:#1161ee;
}

.login-html .sign-in:checked + .tab + .for-pwd + .tab + .login-form .sign-in-htm{
	-webkit-transform:rotate(0);
	transform:rotate(0);
}
.login-html .for-pwd:checked + .tab + .login-form .for-pwd-htm{
	-webkit-transform:rotate(0);
	transform:rotate(0);
}

.hr{
	height:2px;
	margin:60px 0 50px 0;
	background:rgba(255,255,255,.2);
}
.foot-lnk{
	text-align:center;
}
</style>