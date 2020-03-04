## 1.获取粉丝数：
**请求地址：** https://api.live.bilibili.com/relation/v1/Feed/GetUserFc  
**请求类型：** GET  
**参数：**
|  字段   | 必须  | 类型 | 说明 |
|  :----  | :----  | :---- | :---- |
| follow  | 是 | int | 用户UID |

**返回：**
~~~python
{
  "code": 0,
  "msg": "success",
  "message": "success",
  "data": {
    "fc": 67970 # 粉丝数
    }
}
~~~
## 2.获取IP信息：
**请求地址：** https://api.live.bilibili.com/client/v1/Ip/getInfoNew  
**请求类型：** GET  
**参数：** 无  
**返回：**   
~~~python
{
    "code": 0,
    "msg": "",
    "message": "",
    "data": {
        "addr": "47.106.247.232", # IP地址
        "country": "中国", # 国家/地区
        "province": "广东", # 省
        "city": "深圳", # 市
        "isp": "阿里云/电信/联通/移动/铁通/教育网", # 运营商
        "latitude": "22.55516", # 纬度
        "longitude": "114.053879" # 精度
    }
}
~~~

