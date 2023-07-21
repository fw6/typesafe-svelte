<script>
    import SolutionA from "./SolutionA.svelte";
    import SolutionB from "./SolutionB.svelte";
    import SolutionC from "./SolutionC.svelte";
</script>

<SolutionA
    on:open={(e) => console.log(e.detail)}
    on:close={(e) => console.log(e.detail)}
/>

<SolutionB
    on:open={(e) => console.log(e.detail)}
    on:close={(e) => console.log(e.detail)}
/>

<SolutionC
    on:open={(e) => console.log(e.detail)}
    on:close={(e) => console.log(e.detail)}
/>
