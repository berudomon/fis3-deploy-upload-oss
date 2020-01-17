# fis3发布上传静态资源到阿里云oss

fis3 上传静态资源到 阿里云oss 的插件

## 安装

全局安装或者本地安装都可以。

```
npm install fis3-deploy-upload-oss or npm install fis3-deploy-upload-oss -g
```

## 使用方法

使用fis deploy 插件配置
可以配置上传的目录位置

```js
fis.match('*.js', {
    deploy: fis.plugin('alibaba-oss', {
        accessKeyId: '',  //ak
        accessKeySecret: '',  //sk
        bucket: '', //bucket
        region: '', // 默认 oss-cn-hangzhou
        to: '/res-test/frontend/',// 上传的目录位置
    })
})
```