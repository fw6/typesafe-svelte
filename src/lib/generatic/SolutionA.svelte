<script lang="ts" generics="Item">
    import { createEventDispatcher } from "svelte";
    export let items: Item[];

    const dispatcher = createEventDispatcher<{
        close: void;
        open: Item;
    }>();
</script>

<!--
    @component
    typing with generics <script> attribute
    官方推荐方案
    缺点：只能使用有效的通用类型！！！
 -->

{#each items as item}
    <button
        on:click={() => {
            dispatcher("open", item);
        }}
        on:dblclick={() => {
            dispatcher("close");
        }}
    >
        {item}
    </button>
{/each}
