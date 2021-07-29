# AirLine界面说明

## 使用方式

 导包至后台系统web目录下即可

## 数据交互
#### 参数提交： 

  格式：  
  `物品重量：goodsweight，货物长度：goodslength,货物宽度:goodswidth  
  货物高度：goodsheight，货物数量：goodscount，目的地：destination`  
  URL: `paramServlet` 后端接收前台参数所用URL


#### 参数接收：

 格式：json  


 地图：用于航线动态图展示   
 地图参数提前保存为json文件使用时本地读取  
  {
   "airportsFields": [
     "name",
     "city",
     "country",
     "longitude",
     "latitude"
   ],
   "airlineFields": [
     "name",
     "country"
   ],
   "airports": [
     [
       "Goroka",
       "Goroka",
       "Papua New Guinea",
       145.391881,
       -6.081689
     ]
     ]}

  最优报价单：5条最优报价  
  URL: `optimalServlet` 后端向前台发送数据所用URL   
  {
    "optimalprice": [
      "destination",
      "airlines",
      "flightnumber",
      "departure",
      "arrival",
      "timeconsume",
      "transfer",
      "finalprice",
      "remark"
    ]
    }
