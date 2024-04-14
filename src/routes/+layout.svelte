<script>
    import RegularTasks from '../components/RegularTasks.svelte';
    import './styles.css';
</script>

<div class="main">
    <header class="header">
        <div class="main-content header-content">
            <h1 class="app-title">StartYourDay</h1>
        </div>
    </header>
    <slot />
</div>
<RegularTasks />

<style>
    .header-content {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 20px 0;
    }

    .app-title {
        font-family: var(--font-mono);
        font-size: 28px;
        font-weight: 700;
        letter-spacing: 3px;
    }
</style>
