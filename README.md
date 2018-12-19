# txmapapi

腾讯地图 sdk for [腾讯位置服务 WebService API](https://lbs.qq.com/webservice_v1/)

### 一、前期准备

1. 到 (腾讯位置服务控制台)[https://lbs.qq.com/console/key.html] 申请密钥，得到 Key（开发者密钥）


### 三、上传例子

1. 把 demo/lib/* 目录复制到自己项目代码里

2. 在txmapapi.php 中 将申请的Key赋值给 TX_MAP_API_KEY

3. 示例如下
```php
require_once 'lib/txmapapi.php';
$param = [
  'keyword' => '美食',
  'region_fix' => 1,
  'policy' => 0,
  'region' => '常州',
];
$data1 = TxMapApi::getPlaceByKeyword($param);

```

## 说明文档

完整文档有待完善， [使用例子](demo/demo.php)

其他大部分接口可以参考以下 API 文档 [接口文档](https://lbs.qq.com/webservice_v1/)
