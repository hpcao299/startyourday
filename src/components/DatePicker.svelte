<script lang="ts">
    import { DateInput } from 'date-picker-svelte';
    let date = new Date();
    let time = date.getTime() - (date.getTime() % 86400000);
</script>

<DateInput bind:value={date} format="dd-MM-yyyy" placeholder="Choose plan date" />
