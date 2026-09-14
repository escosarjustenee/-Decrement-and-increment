# -Decrement-and-increment
<style>
    body {
        margin: 0;
        min-height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
        background: #0f172a;
        font-family: Verdana, sans-serif;
    }

    .container {
        text-align: center;
        padding: 30px;
    }

    h2 {
        color: #e2e8f0;
        font-size: 30px;
        margin-bottom: 30px;
    }

    button {
        padding: 12px 28px;
        margin: 8px;
        font-size: 17px;
        color: #0f172a;
        background: #cbd5e1;
        border: none;
        border-radius: 6px;
        cursor: pointer;
    }

    button:hover {
        background: #94a3b8;
    }
</style>

<div class="counter-box">

    <h2>Current Number: <span id="number">0</span></h2>

    <button onclick="addNumber()">Add</button>
    <button onclick="subtractNumber()">Subtract</button>

</div>

<script>
    let number = 0;

    function addNumber() {
        number = number + 1;
        document.getElementById("number").textContent = number;
    }

    function subtractNumber() {
        number = number - 1;
        document.getElementById("number").textContent = number;
    }
</script>
