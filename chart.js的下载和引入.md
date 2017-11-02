## Chart.js

# 注意事项（很重要）

- 中文文档是v1.0.0的
- chart.js已经更新到v2+版本

***总结来说***
1. 搜索bootstrap
2. 下拉找到chart.js
3. 点击下载按钮（自动跳转github）
4. 切换到tags  并且版本切换到**v2.0**以下
5. 下载的根目录中只需要 chart.js 和chart.min.js


## 引入Chart.js
```html
<!--min版本为压缩版 体积更小-->
<script src="Chart.min.js"></script>

```

## canvas
```html
<!--输出容器-->
<canvas id="myChart" width="400" height="400"></canvas>

```


### 现在你打开页面可以看到文件引入成功  并且DOM中有一个canvas元素