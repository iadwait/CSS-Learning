<div class="static-box">I am static</div>
<div class="relative-box">I am relative</div>
<div class="container">
    <p>I am normal text</p>
    <button class="absolute-btn">I am absolute</button>
</div>
<div class="fixed-header">I stay on top!</div>
<div class="content">Scroll down to see that the header stays.</div>

<div class="toast">This is a fixed toast notification!</div>

<div class="section">
    <h2 class="sub-header">Section 1</h2>
    <p>Content line 1</p>
    <p>Content line 2</p>
    <p>Content line 3</p>
    <p>Content line 4</p>
    <p>Content line 5</p>
    <p>Content line 6</p>
    <p>Content line 7</p>
    <p>Content line 8</p>
</div>

<div class="section">
    <h2 class="sub-header">Section 2</h2>
    <p>Content line 1</p>
    <p>Content line 2</p>
    <p>Content line 3</p>
    <p>Content line 4</p>
    <p>Content line 5</p>
    <p>Content line 6</p>
    <p>Content line 7</p>
    <p>Content line 8</p>
</div>

<div class="assignment">
    <div class="myContainer">
        <p>
            Assignment Position button to bottom right using position absolute
        </p>
        <button class="btnAssignment">Button</button>
    </div>
</div>

<style>
    .static-box {
        background: #eee;
        padding: 10px;
        margin: 10px;
        border: 1px solid black;
        position: static; /* default */
    }
    .relative-box {
        position: relative;
        top: 20px; /* moves DOWN 20px from normal spot */
        left: 30px; /* moves RIGHT 30px from normal spot */
        background: #cce7ff;
        padding: 10px;
        border: 1px solid #0077cc;
    }
    .container {
        position: absolute; /* sets reference for absolute child */
        border: 1px solid black;
        padding: 20px;
        width: 200px;
        height: 150px;
        top: 10px;
    }
    .absolute-btn {
        position: absolute;
        bottom: 10px;
        right: 10px;
    }
    .fixed-header {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 50px;
        background: #3b82f6;
        color: white;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .content {
        margin-top: 60px; /*so content doesn't hide behind the fixed header */
        height: 1000px;
        background: #f0f0f0;
    }
    .section {
        height: 200px;
        overflow-y: scroll;
        border: 1px solid black;
        margin-bottom: 20px;
        padding: 10px;
    }
    .sub-header {
        position: sticky;
        top: 0; /* sticks to top of section */
        background: #f3f3f3;
        padding: 5px;
        border-bottom: 1px solid #ccc;
    }
    .assignment {
        position: relative;
        border: 2px solid black;
        /* padding: 10px; */
        margin-bottom: 20px;
        height: 150px;
    }
    .myContainer {
        position: absolute;
        top: 10px;
        height: 130px;
        width: 100%;
        background-color: lightcoral;
    }
    .btnAssignment {
        position: absolute;
        bottom: 10px;
        right: 10px;
    }
    .toast {
        position: fixed;
        bottom: 20px; /* distance from bottom of screen */
        right: 20px; /* distance from right of screen */
        padding: 1rem;
        background: #3b82f6;
        color: white;
        border-radius: 5px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        z-index: 10;
    }
</style>
