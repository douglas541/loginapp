<template>
    <div class="container">
        <div class="loginimg">
            <img src="../assets/Loginimg.svg" alt="Login Image">
        </div>
        <div class="logincontent">
            <h1>Uberi</h1>
            <div class="loginwrapper">
                <div class="loginfields">
                    <input type="text">
                    <input type="text">
                </div>
                <button>Login</button>
                <a href="#">Cadastre-se</a>
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
    flex-wrap: wrap;
}

.loginimg img {
    height: 20vw;
    max-height: 500px;
    min-height: 200px;
}

.logincontent {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    /* background-color: red; */

    height: 10vw;
    max-height: 400px;
    min-height: 200px;
    width: 20vw;
    max-width: 600px;
    min-width: 300px;
}

.loginwrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;

    /* background-color: blueviolet; */

    height: 60%;
    width: 80%;
}

.loginfields {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 45%;

    /* background-color: blue; */
}

.loginfields input {
    height: 20px;
    width: 220px;

    border-width: 1px;
    border-radius: 5px;
}
</style>
