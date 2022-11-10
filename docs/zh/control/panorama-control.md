# 全景控件 <Badge type="tip" text="^0.0.31" />

全景地图服务，360°全景地图刻画真实世界，将街道场景带入到地图产品中，用户可以拖拽地图从不同的角度浏览真实的街景效果

```ts
import { PanoramaControl } from 'vue3-baidu-map-gl'
```

:::tip
全景地图服务属于百度地图高级服务，需要向 [百度地图申请](https://lbs.baidu.com/apiconsole/fankui#?typeOne=%E4%BA%A7%E5%93%81%E9%9C%80%E6%B1%82&typeTwo=%E9%AB%98%E7%BA%A7%E6%9C%8D%E5%8A%A1&typeThree=JS%20API%E5%85%A8%E6%99%AF%E5%9B%BE) 才可以使用
:::

## 组件示例

<div>
<Map enableScrollWheelZoom ak='oW2UEhdth2tRbEE4FUpF9E5YVDCIPYih'>
  <PanoramaControl />
  <PanoramaCoverageLayer />
</Map>
</div>

::: details 点击查看代码

<!-- prettier-ignore -->
```html
<Map enableScrollWheelZoom>
  <PanoramaControl />
  <PanoramaCoverageLayer />
</Map>

<script setup lang="ts">
  // PanoramaCoverageLayer 全景图层
  import { Map, PanoramaControl, PanoramaCoverageLayer } from 'vue3-baidu-map-gl'
</script>
```

:::

## 组件事件

| 事件名 | 说明                                       | 类型              |
| ------ | ------------------------------------------ | ----------------- |
| initd  | 组件初始化后，调用的方法，返回一个地图实例 | `{ map, BmapGL, instance }` |
| unload | 组件卸载时会调用此方法                     | -                 |