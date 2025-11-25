<div class="card card1">Card1</div>
<div class="card card2">Card2</div>
<div class="card card3">Card3</div>

<style>
    .card {
        width: 150px;
        height: 100px;
        background: lightblue;
        border: 1px solid black;
        margin: 10px;
        position: relative;
    }
    .card {
        width: 150px;
        height: 100px;
        background: lightblue;
        border: 1px solid black;
        margin: 10px;
        position: relative;
        padding: 10px;
    }
    .card1 {
        top: 0;
        left: 0;
        z-index: 1;
        background: lightcoral;
    }
    .card2 {
        top: -20px;
        left: 20px;
        z-index: 2;
        background: lightsalmon;
    }
    .card3 {
        top: -40px;
        left: 40px;
        z-index: 3;
        background: lightgreen;
    }
</style>
