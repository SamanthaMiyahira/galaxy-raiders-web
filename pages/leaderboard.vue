<template>
    <div class="background-leaderboard">
        <div class="title">
            <h1>Leaderboard</h1>
        </div>
        <div id="leaderboard">
            <table class="leaderboard">
                <tr>
                    <th>Position</th>
                    <th>Score</th>
                    <th>Asteroids Destroyed</th>
                </tr>
                <tr v-for="(score, index) in scores">
                    <td>{{ index+1 }}</td>
                    <td>{{ score.score }}</td>
                    <td>{{ score.asteroidsDestroyed }}</td>
                </tr>
            </table>
        </div>
    </div>
</template>
  
<script>
import leaderboard from "../assets/Leaderboard.json"
export default {
data: () => ({
scores: leaderboard
})
}
</script>

<style scoped>
    .title {
        text-align: center;
        font-size: 20px;
        color: white;
        margin: 20px auto;
    }

    table.leaderboard {
        border-collapse: collapse;
        width: 600px;
        margin: 10px auto;
        background-color: rgba(255, 255, 255, 0.5);
    }

    table.leaderboard td {
        padding: 8px;
        font-size: 16px;
        text-align: center;
        border: 1px solid #ddd;
    }
    
    /*Primeira coluna da tabela*/
    table.leaderboard td:first-child {
        font-weight: bold;
    }

    table.leaderboard th {
        padding: 10px;
        font-size: 18px;
        text-align: center;
        border: 1px solid #ddd;
    }

    *{
        margin: 0;
        padding: 0;
    }

    .background-leaderboard{
        min-height: 100vh;
        display: flex;
        flex-direction: column;
        justify-content: center-up;
        text-align: center-up;
        background-image: url("../assets/bg.jpg");
    }

</style>