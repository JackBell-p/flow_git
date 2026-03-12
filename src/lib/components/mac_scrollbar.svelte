<script lang="ts">
export let height = "100%";
export let width = "100%";
</script>

<div class="mac-scrollbar-root" style="height: {height}; width: {width};">
    <div class="mac-scrollbar-content">
        <slot />
    </div>
</div>

<style>
    .mac-scrollbar-root {
        display: block;
        position: relative;
        overflow-y: auto;
        overflow-x: hidden;
        background: transparent;
     }

    .mac-scrollbar-content {
        display: block;
        width: 100%;
    }

    .mac-scrollbar-root::-webkit-scrollbar {
        width: 12px;
    }

    .mac-scrollbar-root::-webkit-scrollbar-track {
        background: transparent;
    }

    .mac-scrollbar-root::-webkit-scrollbar-thumb {
        background-color: rgba(0, 0, 0, 0.2);
        border-radius: 10px;

        border: 3px solid transparent;
        background-clip: content-box;
        transition: background-color 0.2s;
    }

    .mac-scrollbar-root::-webkit-scrollbar-thumb:hover {
        background-color: rgba(0, 0, 0, 0.4);
    }

    .mac-scrollbar-root::-webkit-scrollbar-thumb:active {
        background-color: rgba(0, 0, 0, 0.5);
    }

    .mac-scrollbar-content::-webkit-scrollbar-button {
        display: none;
    }
</style>
