# lambda-waterLevelTrendAPI

## Overview
現在の降水量の傾向を返します。  
データは10分毎に更新されます。  
データは30分前の傾向データになります。  

## Request
Method : GET  
Endpoint : /production/water-level-trend?country="japan"&prefectures="tokyo"&river="arakawa"  
Parameter :   
1. country : 国名
2. prefectures : 都道府県
3. river : 河川名

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
