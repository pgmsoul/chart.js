# chart.js

基于官方 chart.js 和网友代码，给饼图添加文本显示功能。

### 用法:
```
    <!--饼图（Pie chart）开始-->
    <div>
        <h1>饼图（Pie chart）</h1>
        <canvas id="chart-pie" width="450" height="450"/>
    </div>
    <script>

        var pieData = [
            {
                value: 300,
                color: radom_color(),
                highlight:  radom_color(),
                label: "Red"
            },
            {
                value: 200,
                color:  radom_color(),
                highlight:  radom_color(),
                label: "Green"
            },
            {
                value: 100,
                color:  radom_color(),
                highlight:  radom_color(),
                label: "Yellow"
            },
            {
                value: 400,
                color:  radom_color(),
                highlight:  radom_color(),
                label: "Grey"
            },
            {
                value: 120,
                color:  radom_color(),
                highlight:  radom_color(),
                label: "Dark Grey"
            }
        ];
        var ctx = document.getElementById("chart-pie").getContext("2d");
        //如果每个数据有text属性，显示text属性，如果没有显示 label 属性。
        window.myPie = new Chart(ctx).Pie(pieData);
    </script>

    <!--饼图（Pie chart）结束-->

```
