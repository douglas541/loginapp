<template>
    <div class="container">
        <div class="loginimg">
            <img src="../assets/Loginimg.svg" alt="Login Image">
        </div>
        <div class="logincontent">
            <h1>Olá! Seja bem vindo.</h1>
            <div class="loginwrapper">
                <div class="loginfields">
                    <input type="text" id="username-input" placeholder="username">
                    <input type="password" id="password-input" placeholder="password">
                </div>
                <a href="#" id="login-button">Login</a>
                <a href="#" id="sigin-button">cadastre-se</a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "LoginPage"
}
</script>

<style lang="css" scoped>
.container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    /* flex-wrap: wrap; */

    height: 60vh;
    max-height: 600px;
    min-height: 350px;
    width: 60vw;
    max-width: 1000px;
}

.loginimg {
    display: flex;
    align-items: center;
    justify-content: center;

    border-top-left-radius: 10px;
    border-bottom-left-radius: 10px;
    background-color: #9F99FF;

    height: 100%;
    width: 40%;
}

.loginimg img {
    height: 20vw;
    max-height: 400px;
    min-height: 200px;
}

.logincontent {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;

    background-color: #E7E5FF;

    height: 100%;
    width: 60%;
}

.logincontent h1 {
    margin-bottom: 2rem;

    font-family: sans-serif;
    font-size: 1.2rem;
    font-weight: normal;

    color: #6C63FF;
    width: 60%;
    max-width: 340px;
}

.loginwrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;

    /* background-color: blueviolet; */

    height: 180px;
    width: 60%;
}

.logincontent button {
    width: 6rem;
}

#login-button {
    margin-top: 2rem;

    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #6C63FF;
    width: 120px;
    height: 35px;
    border-radius: 0.3rem;

    font-family: sans-serif;
    font-size: 0.7rem;
    text-decoration: none;
    color: #E7E5FF;
}

#login-button:hover {
    transition: 200ms;
    background-color: #8780FF;
}

#sigin-button {
    font-family: sans-serif;
    font-size: 0.8rem;
    font-weight: normal;
    text-decoration: none;
    color: #6C63FF;
}

.loginfields {
    display: flex;
    flex-direction: column;
    justify-content: space-between;

    height: 60px;
    width: 100%;
    max-width: 340px;

    /* background-color: blue; */
}

.loginfields input {
    height: 20px;
    width: 100%;

    background-color: transparent;

    border: none;
    border-bottom: solid 1px #999999;
    outline: none;
}

.loginfields input::placeholder {
    color: #999999;
}

@media(max-width: 940px) {
    .container {
        width: 70vw;
    }
}

@media(max-width: 820px) {
    .container {
        width: 80vw;
    }
}

@media(max-width: 768px) {
    .container {
        height: 90vh;
        width: 70vw;
        flex-direction: column;
    }

    .loginimg {
        width: 100%;

        border-bottom-left-radius: 0px;
        border-top-right-radius: 10px;
    }

    .logincontent {
        width: 100%;

        border-top-right-radius: 0px;
        border-bottom-left-radius: 10px;
    }
}

@media(max-width: 485px) {
    .container {
        width: 85vw;
    }
}
</style>
