# lambda-waterLevelTrendAPI

## Overview
現在の降水量の傾向を返します。  
データは10分毎に更新されます。  
データは30分前の傾向データになります。  

## Request
Method : GET  
Endpoint : /production/water-level-trend/japan/tokyo/arakawa  
Parameter :   
1. japan : 国名を指定 ex)japan, taiwan  
2. tokyo : 都道府県を指定 ex)tokyo, taipei  
3. arakawa : 河川名を指定 ex)arakawa, danshui  

## Response

以下の Json を返します。
~~~
{
  "timestamp": "2017-08-12T12:50:00",
  "trend": "↑"
}
~~~

timestamp : 分析時点の日時(UTC)  
trend : 降雨量の傾向(↑、↓、→)  
