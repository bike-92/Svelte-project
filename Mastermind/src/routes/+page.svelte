<script>
    import Title from './Title.svelte';

    let showText = false;
    let workingText = 'The button Works';
    function checkSystem() {
        return showText = !showText;
    }
</script>

<Title />

<h1>Hi Alex</h1>
<div>
    <button on:click={checkSystem}>click me!</button>
</div>
{#if showText}
    <p>{workingText}</p>
{/if}