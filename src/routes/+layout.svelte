<script lang="ts">
  
</script>

<div class="container">
  <header class="header">
    <ul>
      <li><a href="/">流量</a></li>
      <li><a href="/log">日志</a></li>
      <li><a href="/about">关于</a></li>
      <li><a href="/donation">打赏</a></li>
    </ul>
  </header>

  <main>
    <slot />
  </main>
</div>

<style>
  @import "./+page.css";
</style>
