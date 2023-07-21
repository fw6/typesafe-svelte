<script>
    import SolutionA from "./SolutionA.svelte";
</script>

<SolutionA>
    <div slot="default" let:id let:title id={id.toString()}>
        <h1>{title}</h1>
    </div>

    <div slot="footer">Footer</div>
</SolutionA>
