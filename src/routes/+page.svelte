<svelte:head>
	<title>ascii brain</title>
	<meta name="description" content="ascii brain - an interactive brain parts diagram for ap psych" />
</svelte:head>

<script lang="ts">
    import { Button } from "$lib/components/ui/button";
    import * as Tabs from "$lib/components/ui/tabs";
</script>

<Tabs.Root value="parts" class="flex flex-col items-center justify-center">
    <Tabs.List>
        <Tabs.Trigger value="parts">parts</Tabs.Trigger>
        <Tabs.Trigger value="lobes">lobes</Tabs.Trigger>
    </Tabs.List>
    <Tabs.Content value="parts">
        <div class="relative">
            <img width="1176" height="1176" src="/images/parts.png" alt="brain" />
            <Button href="/cerebral-cortex" variant="ghost" class="absolute left-[47%] top-[14%] bg-zinc-500 bg-opacity-70 hover:bg-opacity-80 w-[6%] h-[6%] rounded-full"></Button>
            <Button href="/cerebellum" variant="ghost" class="absolute left-[64%] top-[62%] bg-zinc-500 bg-opacity-70 hover:bg-opacity-80 w-[6%] h-[6%] rounded-full"></Button>
            <Button href="/corpus-callosum" variant="ghost" class="absolute left-[42%] top-[33.5%] bg-zinc-500 bg-opacity-70 hover:bg-opacity-80 w-[5%] h-[5%] rounded-full"></Button>
            <Button href="/thalamus" variant="ghost" class="absolute left-[48%] top-[44%] bg-zinc-500 bg-opacity-70 hover:bg-opacity-80 w-[5%] h-[5%] rounded-full"></Button>
            <Button href="/hypothalamus" variant="ghost" class="absolute left-[43%] top-[44.5%] bg-zinc-500 bg-opacity-70 hover:bg-opacity-80 w-[3%] h-[3%] rounded-full"></Button>
            <Button href="/hippocampus" variant="ghost" class="absolute left-[43%] top-[55.5%] bg-zinc-500 bg-opacity-70 hover:bg-opacity-80 w-[3%] h-[3%] rounded-full"></Button>
            <Button href="/amygdala" variant="ghost" class="absolute left-[36%] top-[57%] bg-zinc-500 bg-opacity-70 hover:bg-opacity-80 w-[3%] h-[3%] rounded-full"></Button>
            <Button href="/pons" variant="ghost" class="absolute left-[42.5%] top-[63.5%] bg-zinc-500 bg-opacity-70 hover:bg-opacity-80 w-[5%] h-[5%] rounded-full"></Button>
            <Button href="/medulla" variant="ghost" class="absolute left-[48%] top-[75%] bg-zinc-500 bg-opacity-70 hover:bg-opacity-80 w-[3%] h-[3%] rounded-full"></Button>
            <Button href="/reticular-formation" variant="ghost" class="absolute left-[52.5%] top-[82.5%] bg-zinc-500 bg-opacity-70 hover:bg-opacity-80 w-[4%] h-[4%] rounded-full"></Button>
        </div>
    </Tabs.Content>
    <Tabs.Content value="lobes">
        <div class="relative">
            <img width="1176" height="1176" src="/images/lobes.png" alt="brain" />
            <Button href="/frontal-lobe" variant="ghost" class="absolute left-[25%] top-[25%] bg-zinc-500 bg-opacity-70 hover:bg-opacity-80 w-[6%] h-[6%] rounded-full"></Button>
            <Button href="/parietal-lobe" variant="ghost" class="absolute left-[65%] top-[25%] bg-zinc-500 bg-opacity-70 hover:bg-opacity-80 w-[6%] h-[6%] rounded-full"></Button>
            <Button href="/temporal-lobe" variant="ghost" class="absolute left-[40%] top-[55%] bg-zinc-500 bg-opacity-70 hover:bg-opacity-80 w-[6%] h-[6%] rounded-full"></Button>
            <Button href="/occipital-lobe" variant="ghost" class="absolute left-[85%] top-[45%] bg-zinc-500 bg-opacity-70 hover:bg-opacity-80 w-[6%] h-[6%] rounded-full"></Button>
            <Button href="/brain-stem" variant="ghost" class="absolute left-[50%] top-[70%] bg-zinc-500 bg-opacity-70 hover:bg-opacity-80 w-[4%] h-[4%] rounded-full"></Button>
        </div>
    </Tabs.Content>
</Tabs.Root>
