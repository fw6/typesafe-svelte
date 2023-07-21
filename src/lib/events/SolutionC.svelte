<script>
    import { createEventDispatcher } from "svelte";

    /**
     * @type {import('svelte').EventDispatcher<{ open: 'A' | 'B', close: void; }>}
     */
    const dispatcher = createEventDispatcher();
</script>

<!--
@component

缺点：使用JSDoc，会导致外部使用时，CustomEvent的类型不正确
-->

<button
    on:click={() => dispatcher("open", "A")}
    on:dblclick={() => dispatcher("close")}>Click me</button
>
