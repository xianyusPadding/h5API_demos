# h5API_demos

### demo1 -- baiduMap_api使用

##### 获取 Javascript API 服务方法 
使用百度地图 V2.0版本的引用方式： 
```javascript
<script src="http://api.map.baidu.com/api?v=2.0&ak=yourAppKey" type="text/javascript"></script> （v2.0的版本需要申请密钥（key））
```
##### 创建地图容器元素
地图需要一个 HTML 元素作为容器，这样才能展现到页面上。这里我们创建了一个 div 元素。
##### 命名空间 
API 使用 BMap 作为命名空间，所有类均在该命名空间之下，比如：BMap.Map、BMap.Control、BMap.Overlay。
##### 创建地图实例 
```javascript
var map = new BMap.Map("container"); 
```
位于 BMap 命名空间下的 Map 类表示地图，通过 new 操作符可以创建一个地图实例。其参数可以是元素
id 也可以是元素对象。 
##### 创建点坐标 
```javascript
var point = new BMap.Point(116.404, 39.915); 
```
这里我们使用 BMap 命名空间下的 Point 类来创建一个坐标点。Point 类描述了一个地理坐标点，其中
116.404表示经度，39.915表示纬度。 
##### 地图初始化 
```javascript
map.centerAndZoom(point, 15);   
```
在创建地图实例后，我们需要对其进行初始化，BMap.Map.centerAndZoom()方法要求设置中心点坐标和
地图级别。  地图必须经过初始化才可以执行其他操作。
链接：http://lbsyun.baidu.com/index.php?title=jspopular
