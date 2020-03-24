# hexo-zngw-asset-image
为hexo中的资产图片提供绝对路径

## 说明
这是一个基于[hexo-asset-image ^0.0.5](https://github.com/CodeFalling/hexo-asset-image.git) 版本修改的。原版本中不支持`./about.html`这类网址的生成，新增了图床根目录的配置。

## 安装

```
npm i hexo-zngw-asset-image
```

## 在hexo目录下的_config.yml配置

```yml
imgroot: /					## 配置图床根目录。如果没有图床用本地服务器直接用'/'
post_asset_folder: true		## 需要开启
```

## 例如：
图床目录配置为：
`imgroot: //guoke3915.coding.net/p/guoke3915/d/guoke3915/git/raw/master/`
原文件`/_post/about.html`中有图片`[](about/55.jpg)`
生成的图片路径为`src="//guoke3915.coding.net/p/guoke3915/d/guoke3915/git/raw/master/这里是permalink目录/55.jpg`