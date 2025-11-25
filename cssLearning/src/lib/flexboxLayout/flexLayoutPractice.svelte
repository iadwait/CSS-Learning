<div class="container">
    <div class="card">1</div>
    <div class="card">2</div>
    <div class="card">3</div>
    <div class="card">4</div>
</div>

<style>
    .container {
        display: flex;
        gap: 10px;
        flex-wrap: wrap;
        border: 1px solid black;
        padding: 10px;
    }
    .card:nth-child(1) {
        flex: 1 1 10px;
        background: rgb(167, 94, 94);
    }
    .card:nth-child(2) {
        flex: 1 1 10px;
        background: rgb(84, 45, 45);
    }
    .card:nth-child(3) {
        flex: 1 2 10px;
        background: rgb(167, 94, 94);
    }
    .card:nth-child(4) {
        flex: 1 1 10px;
        background: rgb(147, 62, 62);
    }
</style>
