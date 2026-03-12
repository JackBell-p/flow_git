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
  .container {
    display: grid;
    grid-template-rows: 50px 1fr;
    height: 100vh;
  }

  .header {
    display: flex;
    justify-content: center;
    position: sticky;
    top: 0;
    background: #fff;
    z-index: 2;
  }

  ul {
    list-style-type: none;
    margin: 0px;
    padding: 0px;
    display: flex;
    gap: 20px;
  }

  li {
    font-size: 30px;
  }

  a {
    text-decoration: none;
    color: #000000;
    position: relative;
    padding-bottom: 5px;
    transition: color 0.3s;
  }

  a::after {
    content: "";
    position: absolute;
    width: 80%;
    height: 4px;
    background-color: #00BFFF;
    bottom: 0px;
    left: 10%;
    border-radius: 2px;
    opacity: 0;
    transition: opacity 0.3s;
  }

  a:hover,
  a.active {
    color: #00BFFF;
  }

  a:hover::after,
  a.active::after {
    opacity: 1;
  }

  main {
    background-color: #ececec;
    overflow-y: auto;
  }

</style>
