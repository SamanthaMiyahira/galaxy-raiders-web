<template>
    <div class="background-index">
        <div class="title">
            <h1>Galary Raiders</h1>
        </div>
        <button class="button button1"><NuxtLink to="jogo">Iniciar Partida</NuxtLink></button>
        <button class="button button2"><NuxtLink to ="leaderboard">Leaderboard</NuxtLink></button>
        <button class="button button3"><NuxtLink to ="saida">Sair</NuxtLink></button>
    </div>
</template>
  
<script>
</script>

<style scoped>
    .title {
        text-align: center;
        font-size: 20px;
        color: white;
        margin: 20px auto;
    }

    .button {
        border: none;
        color: white;
        padding: 16px 32px;
        text-align: center;
        text-decoration: none;
        display: inline-block;
        font-size: 16px;
        margin: 10px 550px;
        transition-duration: 0.4s;
        cursor: pointer;
        text-color: black;
    }

    .button1 {
        background-color: white; 
        color: black; 
        border: 2px solid #429853;
    }

    .button1:hover {
        background-color: #429853;
        color: white;
    }

    .button2 {
        background-color: white; 
        color: black; 
        border: 2px solid #0A579A;
    }

    .button2:hover {
        background-color: #0A579A;
        color: white;
    }

    .button3 {
        background-color: white; 
        color: black; 
        border: 2px solid #CB142D;
    }

    .button3:hover {
        background-color: #CB142D;
        color: white;
    }

    *{
        margin: 0;
        padding: 0;
    }

    .background-index{
        min-height: 100vh;
        display: flex;
        flex-direction: column;
        justify-content: center-up;
        text-align: center-up;
        background-image: url("../assets/menu2.jpg");
    }

</style>