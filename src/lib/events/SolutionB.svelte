<script lang="ts">
    import { createEventDispatcher } from "svelte";

    interface $$Events {
        open: CustomEvent<"A" | "B" | "C">;
        close: CustomEvent<void>;
    }

    const dispatcher = createEventDispatcher();
</script>

<button
    on:click={() => dispatcher("open", "A")}
    on:dblclick={() => dispatcher("close")}>Click me</button
>
