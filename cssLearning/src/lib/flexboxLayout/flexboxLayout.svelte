<script>
    let selectedOption = 'home';
    import FlexboxAdvanced from "$lib/flexboxAdvanced/flexboxAdvanced.svelte";
    import FlexboxBasics from "$lib/flexboxBasics/flexboxBasics.svelte";
</script>

<div class="layout">
    <aside class="sidebar">
        <button on:click={() => selectedOption='home'}>Home</button>
        <button on:click={() => selectedOption='about'}>About</button>
    </aside>
    <main class="content">
        {#if selectedOption === 'home'}
            <p>This is Home Page</p>
            <FlexboxAdvanced />
        {:else if selectedOption === 'about'}
            <p>This is About Page</p>
            <FlexboxBasics />
        {/if}
    </main>
</div>

<style>
    .layout {
        display: flex;
        height: 100vh;
    }
    .sidebar {
        width: 250px;
        background: #f0f0f0;
        padding: 20px;
    }
    .content {
        flex: 1;
        background: white;
        padding: 20px;
    }
    /* For small device like mobile less than 600px width */
    @media (max-width: 600px) {
        .layout {
            flex-direction: column;
        }

        .sidebar {
            width: 100%;
        }
    }
</style>
