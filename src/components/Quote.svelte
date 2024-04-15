<script>
    // @ts-ignore
    import SvelteTooltip from 'svelte-tooltip';
</script>

<div class="quote-wrapper">
    <SvelteTooltip tip="Click to change quote" bottom color="#333"
        ><div class="quote">There is nothing to do today. Bro!</div>
    </SvelteTooltip>
</div>

<style>
    .quote-wrapper {
        color: #fafafa;
    }

    .quote {
        font-size: 56px;
        font-weight: 700;
        color: var(--color-text);
        cursor: pointer;
    }
</style>
