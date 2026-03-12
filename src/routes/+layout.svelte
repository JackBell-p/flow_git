<script lang="ts">
  import { page } from "$app/state";
  import Mac_Scrollbar from "$lib/components/mac_scrollbar.svelte";

  const nav_items = [
    { path: "/", lable: "流量"},
    { path: "/log", lable: "日志"},
    { path: "/about", lable: "关于"},
    { path: "/donation", lable: "打赏"}
  ];
</script>

<div class="container">
  <header class="header">
    <ul>
      {#each nav_items as item}
        <li><a href={item.path} class={page.url.pathname === item.path ? 'active' : ''}>{item.lable}</a></li>
      {/each}
    </ul>
  </header>

  <main>
    <Mac_Scrollbar>
      <slot />
    </Mac_Scrollbar>
  </main>
</div>

<style>
  @import "./+layout.css";
</style>
