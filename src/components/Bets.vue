<template>
    <table>
        <tr>
            <td>Ticket</td>
            <td>Amount</td>
            <td>Result</td>
            <td>Winning</td>
        </tr>
        <tr v-for="bet in bets" :key="bet.id" class="bet" :class="bet.result">
            <td>{{bet.title}}</td>
            <td>{{bet.amount}}</td>
            <td>{{bet.result}}</td>
            <td>{{bet.winning}}</td>
        </tr>
        <tr>
            <td>Total</td>
            <td id="total">{{total}}</td>
        </tr>
    </table>
</template>

<script>

    export default {
        name: 'Bets',
        props: {
            bets: Array
        },
        computed: {
            total() {
                let total = 0
                for (let bet of this.bets) {
                    if (bet.result === 'win') {
                        total += bet.winning
                    } else {
                        total -= bet.amount
                    }
                }

                return total
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    table{
        width: 50%;
        margin: 0 auto;
    }
    h3 {
        margin: 40px 0 0;
    }

    ul {
        list-style-type: none;
        padding: 0;
    }

    li {
        display: inline-block;
        margin: 0 10px;
    }

    a {
        color: #42b983;
    }
    .win {
        color: #42b983;
    }
    .lose {
        color: #b91700;
    }
</style>