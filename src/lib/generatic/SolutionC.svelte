<script>
    /**
     * @template {{id: number; name: string}} Item
     * @type {Item[]}
     */
    export let list;
</script>

<!--
    @component
    typing with JSDoc

    实验性质，无法使用！
 -->

{#each list as item}
    {item}
{/each}
