# 2019KDD_EXTERANL_DATA
external data about location data

  
  百度地图API逆向地理位置编码数据，数据掉用自百度API，使用2019年KDDCUP赛事中训练集合测试集对应所有'o','d'坐标数据的逆地理位置编码
---------------------

0-0-1:更新
根据论坛问题，坐标不对情况进行了改进，添加W4G参数获得以获得正确的地理位置数据，参考文档API：http://lbsyun.baidu.com/index.php?title=webapi/guide/webservice-geocoding-abroad
爬虫使用链接公式：
url = "http://api.map.baidu.com/geocoder/v2/?callback=renderReverse&location={},{}&output=json&pois=0&latest_admin=1&coordtype=wgs84ll&ak={}".format(latitude,longitude,youAK)
youAK:API的开发者AK密钥
