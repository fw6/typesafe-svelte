<script lang="ts">
    interface $$Slots {
        default: {
            id: number;
            title: string;
        };
        footer: {};
    }
</script>

<slot id={1} title={"Lily"}>Main</slot>
<slot name="footer">footer</slot>
