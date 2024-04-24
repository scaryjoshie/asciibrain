<script lang="ts">
    import { Button } from "$lib/components/ui/button";
    import Arrow from "lucide-svelte/icons/corner-down-left"

    export let name: string;
    export let definition: string;
</script>

<div class="flex flex-col items-center justify-center gap-16">

    <h1 class="text-2xl">{name}</h1>

    <p>{definition}</p>

    <Button variant="outline" href="/">
        go back
        <Arrow class="ml-4 h-4 w-4" />
    </Button>

</div>
