# 使用

地图采用天地图全国地级市层面边界数据。

## 样式切换

自己定义 `RGB` 并切换即可。

```js
let blackStyle = [
   "#343233",  // 背景和省份颜色
   "#2be4f3",  // 省份边界线颜色
   "#5aae5c",  // 点亮省份的颜色
   "#fff",     // 标签字体的颜色
   "#ffff00"   // 城市圆点的颜色
];
let grayStyle = [
   "#dedfde",
   "#6e6e6d",
   "#d5e5f1",
   "#000",
   "#fe7e3a",
]

// 自由选择样式
let style = grayStyle;
```

## 点亮城市

在 `regions` 添加字段即可。

```js
regions: [
   { name: "金华市", itemStyle: { normal: { areaColor: style[2] } } },
   { name: "杭州市", itemStyle: { normal: { areaColor: style[2] } } },
   { name: "嘉兴市", itemStyle: { normal: { areaColor: style[2] } } },
   { name: "宁波市", itemStyle: { normal: { areaColor: style[2] } } },
   { name: "绍兴市", itemStyle: { normal: { areaColor: style[2] } } },
   { name: "丽水市", itemStyle: { normal: { areaColor: style[2] } } },
   { name: "上海市", itemStyle: { normal: { areaColor: style[2] } } },
   { name: "北京市", itemStyle: { normal: { areaColor: style[2] } } },
   { name: "重庆市", itemStyle: { normal: { areaColor: style[2] } } },
   { name: "深圳市", itemStyle: { normal: { areaColor: style[2] } } },
   { name: "广州市", itemStyle: { normal: { areaColor: style[2] } } },
   { name: "佛山市", itemStyle: { normal: { areaColor: style[2] } } },
   { name: "珠海市", itemStyle: { normal: { areaColor: style[2] } } },
   { name: "厦门市", itemStyle: { normal: { areaColor: style[2] } } },
   { name: "香港特别行政区", itemStyle: { normal: { areaColor: style[2] } } },
   { name: "澳门特别行政区", itemStyle: { normal: { areaColor: style[2] } } },
   { name: "台湾省", itemStyle: { normal: { areaColor: style[2] } } },
],
```

## 去过的城市

添加经纬度即可。

```js
 data: [
   { name: '北京', value: [116.407387, 39.904179] },
   { name: '长白山', value: [128.333, 42.026] },
   { name: '武当山', value: [110.785239, 32.647017] },
   { name: '保定', value: [115.482331, 38.867657] },
   { name: '唐山', value: [118.460379, 39.273070] },
   { name: '天津', value: [117.190182, 39.125596] },
   { name: '秦皇岛', value: [119.586579, 39.942531] },
   { name: '乌兰布统', value: [117.54562, 43.26501] },
   { name: '张家口', value: [115.27993, 40.97519] },
   { name: '成都', value: [104.04303, 30.64235] },
   { name: '西宁', value: [101.778916, 36.623178] },
   { name: '长沙', value: [112.93133, 28.2351] },
   { name: '南昌', value: [115.892151, 28.676493] },
   { name: '武功山', value: [114.02951, 27.63063] },
   { name: '黄山', value: [118.1416, 30.2729] },
   { name: '洛阳', value: [112.46902, 34.68364] },
   { name: '敦煌', value: [94.66159, 40.14211] },
   // { name: '黟县', value: [117.94137, 29.92588] },
   { name: '西安\n 咸阳', value: [108.94866, 34.22245] },
   { name: '华山', value: [110.08752, 34.56608] },
   { name: '延安', value: [110.17196, 36.04732] },
   { name: '宝鸡', value: [107.90017, 34.37524] },
   // { name: '咸阳', value: [108.705117, 34.333439] },
   { name: '九寨沟县', value: [104.231374, 33.279792] },
   { name: '茶卡镇', value: [98.48196, 36.93471] },
   { name: '张掖', value: [100.455472, 38.932897] },
   { name: '格尔木', value: [94.90329, 36.40236] },
   { name: '衡山', value: [112.86776, 27.23134] },
],
```

## 预览

``` python
python3 -m http.server
```