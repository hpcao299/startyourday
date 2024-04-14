<script lang="ts">
    import DatePicker from '../components/DatePicker.svelte';
    import Quote from '../components/Quote.svelte';
    import TodoList from '../components/TodoList.svelte';
</script>

<div class="content">
    <div class="quote-wrapper">
        <Quote />
    </div>

    <div class="split-content">
        <div class="content-item">
            <TodoList />
        </div>
        <div class="content-item"></div>
    </div>
</div>

<style>
    .content {
        padding-top: 56px;
    }

    .quote-wrapper {
        padding-bottom: 32px;
        margin-bottom: 64px;
        border-bottom: 1px solid #ccc;
    }

    .split-content {
        display: flex;
        gap: 28px;
    }

    .content-item {
        width: 50%;
        flex: 50%;
        padding: 0 24px;
    }
</style>
