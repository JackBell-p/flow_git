<script lang="ts">
    let logs = [
        { timestamp: "2026-03-03 23:29:50.285", level: "error", message: "dns拦截器异常" },
        { timestamp: "2026-03-03 23:29:50.199", level: "info", message: "FastGithub 启动完成，当前版本为 V2.1.5" },
        { timestamp: "2026-03-03 23:29:50.126", level: "info", message: "已监听 git://localhost:9418，github 的 git 反向代理服务启动完成" },
        { timestamp: "2026-03-03 23:29:50.124", level: "info", message: "已监听 ssh://localhost:22，github 的 ssh 反向代理服务启动完成" },
        { timestamp: "2026-03-03 23:29:50.061", level: "info", message: "已监听 http://localhost:80，http 反向代理服务启动完成" },
        { timestamp: "2026-03-03 23:29:49.990", level: "info", message: "已监听 https://localhost:443，https 反向代理服务启动完成" }
    ];

    let seleted_index: number;

    function select_log(index: number) {
        seleted_index = index;
    }
</script>

<div class="log-container">
  {#each logs as log, i}
    <button class="log-entry {log.level} {seleted_index === i ? 'selected' : ''}" on:click={() => select_log(i)}>
      <span class="time">{log.timestamp}</span>
      <span class="level">[{log.level.toUpperCase()}]</span>
      <span class="message">{log.message}</span>
    </button>
  {/each}
</div>

<style>
    @import "./+page.css";
</style>
