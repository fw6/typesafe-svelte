<script lang="ts">
    import { createEventDispatcher } from "svelte";

    const dispatcher = createEventDispatcher<{
        close: void;
        open: "A" | "B" | "C";
    }>();
</script>

<!--
@component
Typing events

给事件添加类型，在监听定义事件之外的任何事件都会报错

-->

<button
    on:click={() => dispatcher("open", "A")}
    on:dblclick={() => dispatcher("close")}>Click me</button
>
