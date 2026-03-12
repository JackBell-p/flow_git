<script lang="ts">
    import { onMount } from "svelte";
    import * as echarts from "echarts";

    let chart_div: HTMLDivElement;

    onMount(() => {
        const chart = echarts.init(chart_div);

        chart.setOption({
            title: { text: "网络流量监控" },
            tooltip: { trigger: "axis" },
            legend: { data: ["上行流量", "下行流量"] },
            xAxis: {
                type: "category",
                data: ["08:00:00", "08:05:00", "08:10:00", "08:15:00"]
            },
            yAxis: {
                type: "value",
                name: "B/s",
                min: 0,
                max: 18
            },
            series: [
                {
                    name: "上行流量",
                    type: "line",
                    data: [0, 2, 4, 0],
                    color: "blue",
                    smooth: true
                },
                {
                    name: "下行流量",
                    type: "line",
                    data: [0, 5, 10, 0],
                    color: "red",
                    smooth: true
                }
            ]
        });

        window.addEventListener("resize", () => chart.resize());
    });
</script>

<div bind:this={chart_div} class="chart"></div>

<style>
    .chart {
        width: 100%;
        height: 100%;
        overflow: hidden;
    }
</style>
