<div class="container">
    <div class="card">Card 1</div>
    <div class="card">Card 2</div>
    <div class="card">Card 3</div>
    <div class="card">Card 4</div>
    <div class="card">Card 5</div>
    <div class="card">Card 6</div>
    <div class="card">Card 7</div>
</div>

<style>
    .container {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 20px;
        padding: 20px;
    }
    .card {
        background: #d88989;
        padding: 20px;
        border-radius: 10px;
        width: 350px;
        /* flex: grow shrink basis */
        flex: 1 1 250px; 
        /* min-width: 250px; */
    }
</style>