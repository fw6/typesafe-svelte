<script lang="ts">
    interface $$Props {
        name: string;
        age?: number;
        male?: boolean;
    }

    export let name: string;
    export let age = 18;
</script>

name: {name}
age: {age}

restProps: {JSON.stringify($$restProps)}
props: {JSON.stringify($$props)}
