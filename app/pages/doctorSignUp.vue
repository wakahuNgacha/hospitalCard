<template>
    <div class="holder">
        <div class="left">
            <div class="formHolder">
                <div>
                    <div class="logo">
                        <h3>Hospital Card</h3>
                    </div>
                    <div class="title">
                        <h1>Hey</h1>
                        <h1>Nice to see you!</h1>
                    </div>
                    <div class="subtitle">
                        <h3>Sign in to get all your patient's medical records in one place</h3>
                    </div>
                </div>

                <div class="form">
                    <form action="" method="post">

                        <div class="formgroup">
                            <label for="username">Your name</label>
                            <input type="text" id="name" name="name" v-model="name" placeholder="username" required>
                        </div>

                        <div class="formgroup">
                            <label for="email">Email</label>
                            <input type="email" id="email" name="email" v-model="email" placeholder="example@company.com" required>
                        </div>
                        <div class="formgroup">
                            <label for="password">Password</label>
                            <input type="password" id="password" name="password" v-model="password" placeholder="••••••••" required>
                        </div>
                        <div class="formgroup" id="forgot">
                            <div>
                                <input type="checkbox" id="remember" name="remember">
                                <label for="remember">Remember Me</label>                                
                            </div>

                        </div>
                        <div class="formgroup">
                            <button type="submit">Sign In</button>
                        </div>
                    </form>
                </div>
                
                <div class="formgroup">
                    <span>Alredy have an account? <NuxtLink to="/doctorLogIn">Log in</NuxtLink></span>
                </div>
            </div>
        </div>
        <div class="right">
            <img src="/nurse.jpg" alt="Image of a doctor and patient">
        </div>        
    </div>

</template>
<script setup> </script>
<style scoped>
.holder {
    height: 98vh;
    width: 98vw;
    border-radius: 20px;
    border: 1px solid rgb(214, 214, 214);
    background-color: white;
    display: flex;
    flex-direction: row;
}
.left {
    width: 50%;
    height: 100vh;
    float: left;
    display: flex;
    justify-content: center;
    align-items: center;
    /* background-color: blue; */
}
.right {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 50%;
    height: 98vh;
    float: right;
    /* background-color: lightpink; */
}
.right img {
    width: 96%;
    height: 96%;
    object-fit: cover;
    border-radius: 10px;
}
.formHolder {
    width: 70%;
    height: 90%;
    /* background-color: lightgray; */
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: start;
}
.logo {
    margin-bottom: 50px;
}
.form{
    width: 80%;
}
.formgroup {
    width: 100%;
    margin-bottom: 15px;
    display: flex;
    flex-direction: column;
}
input[type="email"], input[type="password"], input[type="text"] {
    width: 100%;
    padding: 10px;
    margin-top: 5px;
    border: 1px solid #ccc;
    border-radius: 5px;
    box-sizing: border-box;
}
#forgot {
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
}
a {
    text-decoration: none;
    color: var(--accent);
}
</style>