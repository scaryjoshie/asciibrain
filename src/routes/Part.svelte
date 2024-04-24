<script lang="ts">
    import { Button } from "$lib/components/ui/button";

    export let name: string;
    export let definition: string;
</script>

<div class="flex flex-col items-center justify-center gap-16">

    <h1 class="text-2xl">{name}</h1>

    <p>{definition}</p>

    <Button variant="ghost" href="/">
        go back
    </Button>

</div>
