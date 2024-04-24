<script lang="ts">
    import "../app.css";

    import Header from "./Header.svelte";
    import Sidebar from "./Sidebar.svelte";
</script>

<div class="flex flex-col items-center gap-16">

    <Header />

    <div class="flex flex-row justify-center gap-8 w-full max-w-[108rem] px-16">
        <div class="basis-1/6">
            <Sidebar />
        </div>
        <div class="basis-2/3">
            <slot />
        </div>
        <div class="basis-1/6"></div>
    </div>

</div>
