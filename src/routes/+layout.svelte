<script lang="ts">
    import "../app.css";

    import Header from "./Header.svelte";
    import Sidebar from "./Sidebar.svelte";
</script>

<div class="flex flex-col items-center gap-16">

    <Header />

    <div class="flex flex-col md:flex-row max-md:items-center justify-center gap-8 w-full max-w-[108rem] md:px-16">
        <div class="order-2 md:order-1 md:basis-1/6">
            <Sidebar />
        </div>
        <div class="order-1 md:order-2 md:basis-2/3">
            <slot />
        </div>
        <div class="max-md:hidden md:order-3 basis-1/6"></div>
    </div>

</div>
