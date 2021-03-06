# data-visualization
数据可视化：基于d3.js 或 fabric.js 等

## 市场图表

> 个人经验：
>
> 偏展现场景，建议优先采用类置标语言（Markup Language）的类库，直观；偏交互场景，选用易编程、易定制的类库。

### 偏展现图表

| 图表                                       | 特点                                       |
| ---------------------------------------- | ---------------------------------------- |
| [Echarts](http://echarts.baidu.com/index.html) |                                          |
| [AntV](https://antv.alipay.com)          | 蚂蚁金服全新一代数据可视化解决方案。包括[可视化图形语法库 G2](https://github.com/antvis/g2/)、 [流程图和关系分析的G6](https://github.com/antvis/g6/)、 [面向移动端的可视化图形语法库 F2](https://github.com/antvis/f2) |
| [Viserjs](https://github.com/viserjs/viser) | 基于 [G2](https://github.com/antvis/g2) 的图形库，置标语言（ Markup Language）使用方式，支持 React、Angular 和Vue，由 [Recharts](https://github.com/recharts/recharts) 等成员开发 |
| [Recharts](https://github.com/recharts/recharts) | 对 React 和 D3 的封装，置标语言（ Markup Language）使用方式，对 React 支持友好，由 Alibaba 成员发起 |
| [Frappé Charts](https://github.com/frappe/charts) | 基于 SVG                                   |
| [SVG.js](https://github.com/svgdotjs/svg.js) | 将 SVG 的置标语言使用方式封装成了一套类似 Canvas （或 D3）的 APIs，增强了 SVG 的交互开发体验 |
| [Vega](https://vega.github.io/vega/)     |                                          |
| [Vega-Lite](https://vega.github.io/vega-lite/) |                                          |

### 偏交互图表

| 图表                                       | 特点                                       |
| ---------------------------------------- | ---------------------------------------- |
| [AntG](http://antg.alipay.net/)          | 3D 图形方向。蚂蚁金服在互联网交互图形领域的探索沉淀，包括 [R3](http://antg.alipay.net/r3/getting-started-cn) 和 [WebAR](http://antg.alipay.net/webar/introduction-cn)。著名应用有蚂蚁庄园、小鸡快跑等。 |
| [Fabric.js](http://fabricjs.com/)        |                                          |
| [konva](http://konvajs.github.io/)       |                                          |
| [D3](https://d3js.org/)                  |                                          |
| [JavaScript InfoVis Toolkit](https://github.com/philogb/jit) |                                          |
| [Protovis](http://mbostock.github.io/protovis/ex/) | D3.js 前身，使用SVG的可视化JS。从后续发展看，不建议在新项目中采用。如重新设计新可视化JS，可参考。 |

### 其它

| 图表                                       | 特点                                       |
| ---------------------------------------- | ---------------------------------------- |
| [Deck.gl](https://github.com/uber/deck.gl) | Uber 的一个 WebGL 大规模数据展现库。其他还有 [luma.gl](https://uber.github.io/luma.gl/#/)、[react-vis](https://uber.github.io/react-vis/)、[react-map-gl](https://uber.github.io/react-map-gl/) |
| [Planck.js](https://github.com/shakiba/planck.js) | 2D 物理引擎                                  |
| [whs.js](https://github.com/WhitestormJS/whs.js) | 基于Three.js，适用于 Web 应用程序与游戏的3D框架          |
| [Embedding Projector](https://www.tensorflow.org/get_started/embedding_viz) | 谷歌开源的高维数据可视化                             |
| [Phaser](https://github.com/photonstorm/phaser) | HTML5 Game Framework                     |
| [AnyPixel.js](http://googlecreativelab.github.io/anypixel) | 谷歌，个人认为比较适合交互式大屏                         |
| [LayerVisualizer](https://github.com/romannurik/LayerVisualizer) | 一个简单的基于Web的3D图层（可用于可视化材质UI和涉及深度/阴影的其他事物） |


## 项目

### 图片标定

calibrationbox：一个 [Fabric](http://fabricjs.com/) 的小插件，可用于标定图片中车辆、人、交通灯标识、区域等。详见，[calibration-box](https://github.com/TingGe/calibration-box) 项目。

![](https://github.com/TingGe/calibration-box/raw/master/assets/calibrationbox.png)

### 网络攻击地图

- norsecorp

![](./assets/norsecorp.png)

- ipviking

  ![](./assets/ipviking.png)

### 访问者流报告

netflow：借鉴 Google Analytics 行为流 ，修改自 [netFlow](https://github.com/jdk137/netFlow/)

![](./assets/netflow.png)

## 运行

1. 依赖 [Node](https://nodejs.org/)、[http-server](https://github.com/indexzero/http-server)
2. 在 data-visualization/server 目录执行 `npm install` 后，运行 `npm start` 启动（默认9999端口）
3. 在 data-visualization 目录执行 `http-server`
4. 根据 `http-server` 中提示的网址，在浏览器（建议 Chrome ）中访问
5. 关闭命令窗口即可退出

## 附录

- [数据可视化工具目录](http://www.datavizcatalogue.com/ZH/index.html)
- [Sankey Diagrams](https://bost.ocks.org/mike/sankey/)
- [读书笔记 - 数据可视化实践](http://blog.lyuehh.com/book/2013/05/25/reading-notes-Interactive-Data-Visualization.html)
- [F1 Championship Points as a d3.js Powered Sankey Diagram](https://blog.ouseful.info/2012/05/24/f1-championship-points-as-a-d3-js-powered-sankey-diagram/)
- [前端模块化开发DEMO之攻击地图](http://fuxiaode.cn/blog/2015/12/05/attack-map-with-amd)：推荐 @[依宁](https://github.com/danislyn) 的一版[攻击地图](http://fuxiaode.cn/demo/AttackMap/index.html)，感觉不错！
- [konva](http://konvajs.github.io/)：呈现能力不错，但与  [Fabric](http://fabricjs.com/) 相比交互较弱。

## 反馈

[https://github.com/TingGe/data-visualization/issues](https://github.com/TingGe/data-visualization/issues)

## 贡献

[https://github.com/TingGe/data-visualization/graphs/contributors](https://github.com/TingGe/data-visualization/graphs/contributors)

## 许可

(The MIT License)

Copyright (c)  Ting Ge [505253293@163.com](mailto:505253293@163.com)

