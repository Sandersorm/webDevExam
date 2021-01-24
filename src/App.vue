<template>
    <div id="app">
        <Bets :bets="data"/>
    </div>
</template>

<script>
    import Bets from './components/Bets.vue'

    export default {
        name: 'App',
        components: {
            Bets
        },
        data: function () {
            return {
                data: [
                    {
                        id: 1,
                        title: "Bet #1",
                        amount: 200,
                        result: "win",
                        winning: 400
                    },
                    {
                        id: 2,
                        title: "Bet #2",
                        amount: 1500,
                        result: "lose"
                    },
                    {
                        id: 3,
                        title: "Bet #3",
                        amount: 500,
                        result: "win",
                        winning: 870
                    },
                    {
                        id: 4,
                        title: "Bet #4",
                        amount: 350,
                        result: "win",
                        winning: 690
                    },
                ]
            }
        }
    }
</script>

<style>
    #app {
        font-family: Avenir, Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }
</style>