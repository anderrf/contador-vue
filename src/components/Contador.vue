<template>
    <div class="contador">
        <h1>Contador</h1>
        <div>
            <p>Valor atual: <span :class="contagem < 0 ? 'text-red' : ''">{{contagem}}</span></p>
            <div class="btnDiv">
                <button type="button" id="btnDec" @click="decrementar">-</button>
                <button type="button" id="btnInc" @click="incrementar">+</button>
            </div>
        </div>
    </div>
</template>
<script>
    export default{
        name: 'Contador',
        data(){
            return{
                contagem: 0
            }
        },
        methods: {
            incrementar(){
                this.contagem++;
            },
            decrementar(){
                this.contagem--;
            }
        }
    }
</script>
<style scoped>
    .contador{
        display: flex;
        flex-direction: column;
    }

    .contador h1{
        text-align: center;
        margin: 10px auto 50px;
    }

    .contador > div{
        text-align: center;
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .btnDiv{
        width: 80%;
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        margin: 20px auto;
    }

    .btnDiv button{
        font-size: 1em;
        font-family: Tahoma;
        width: 2em;
        height: 2em;
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
        border: none;
        outline: none;
        cursor: pointer;
        color: #FFFFFF;
        font-weight: bolder;
    }

    #btnDec{
        background-color: #0000FF;
    }

    #btnInc{
        background-color: #00FF00;
    }

    .text-red{
        color: #FF0000;
    }
</style>