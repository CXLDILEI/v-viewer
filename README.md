# `v-viewer`

> 基于viewerjs开发的vue图片预览组件

## Usage

```
improt VViewer from 'v-viewer'
```


```
<viewer ref="viewer" :options="options" :images="images" @inited="inited" @hidden="hidden">
    <img
      v-for="item in images"
      :key="item.url"
      :data-original="item.url"
      :src="item.url"
      :alt="item.fileName"
    />
</viewer>

private $viewer: any = null
private inited(viewer) {
  // 暴露viewer实例
  this.$viewer = viewer
}
```

## Methods & Options

配置项及方法参考viewerjs:

[https://github.com/fengyuanchen/viewerjs/blob/master/README.md](https://)
