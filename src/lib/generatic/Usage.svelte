<script lang="ts">
    import SolutionA from "./SolutionA.svelte";
    import SolutionB from "./SolutionB.svelte";
    import SolutionC from "./SolutionC.svelte";
</script>

<!-- SolutionA -->
<SolutionA items={[]} />
<SolutionA items={[true, false]} />
<SolutionA items={["a", "b"]} />
<SolutionA items={[1, 2]} />

<!-- SolutionB -->
<SolutionB items={[]} list={[]} />
<SolutionB items={[true, false]} list={[{ id: 1, name: "Lily" }]} />
<SolutionB items={["a", "b"]} />
<SolutionB items={[1, 2]} />

<SolutionC list={[]} />
<!--
<SolutionC list={[true, false]} />
<SolutionC list={["a", "b"]} />
<SolutionC list={[1, 2]} />
-->
