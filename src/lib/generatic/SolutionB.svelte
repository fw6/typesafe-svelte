<script lang="ts">
    type Item = $$Generic;
    type Item2 = $$Generic<{ id: Number; name: string }>;

    export let items: Item[];
    export let list: Item2[] | undefined = undefined;
</script>

<!--
    @component
    @deprecated
    typing with $$Generic

    废弃语法！但目前还可使用
    缺点：使用`const T extends string`等高级类型时无效
 -->

{#each items as item}
    {item}
{/each}
{#if list}
    {#each list as item}
        {item.id} {item.name}
    {/each}
{/if}
