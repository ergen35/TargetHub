<script>
    import { navigating } from '$app/stores'
    import { Loading } from "attractions";

	export let data;
</script>


<div class="container-fluid">
    {#if $navigating}
         <!-- content here -->
        <div class="nav-preloader">
            <Loading />
            Loading..
        </div>
    {:else}
         <!-- else content here -->
         <slot></slot>
    {/if}
</div>

<style>
    div.nav-preloader{
        top: 50%;
        left: 50%;
        position: absolute;
    }
</style>