<script>
    let open = false;
</script>

<nav>
    <div>Logo</div>

    <div class="hamburger" on:click={() => (open = !open)}>
        {#if open}
            ✖
        {:else}
            ☰
        {/if}
    </div>

    <ul class:show={open}>
        <li>Home</li>
        <li>About</li>
        <li>Contact</li>
    </ul>
</nav>

<style>
    nav {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0 20px;
        height: 60px;
        background: #f5f5f5;
        position: relative;
    }
    nav ul {
        display: flex;
        gap: 20px;
        list-style: none;
        margin: 0;
        padding: 0;
    }
    nav ul li {
        cursor: pointer;
        font-size: 16px;
        transition: color 0.2s ease;
    }
    nav ul li:hover {
        color: #007aff; /* iOS blue */
    }

    /* Hamburger hidden on desktop */
    .hamburger {
        font-size: 28px;
        cursor: pointer;
        display: none;
    }

    @media (max-width: 600px) {
        nav ul {
            display: none;
            flex-direction: column;
            background: #f5f5f5;
            position: absolute;
            top: 60px;
            right: 0;
            width: 150px;
            padding: 15px 0;
        }

        nav ul.show {
            display: flex;
        }

        .hamburger {
            display: block;
        }
    }
</style>
