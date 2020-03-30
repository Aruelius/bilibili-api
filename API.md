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
## 2.获取 IP 信息：
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

## 3. 通过 BVID 查询稿件信息

**请求地址：** https://api.bilibili.com/x/web-interface/archive/stat   

**请求类型：**GET  

**参数：  **

| 字段 | 必须 | 类型 | 说明         |
| ---- | ---- | ---- | ------------ |
| bvid | 是   | int  | 视频 BVID 号 |

**返回： ** 

~~~json
{
    "code":0,
    "message":"0",
    "ttl":1,
    "data":{
        "aid":242572847, # 视频 aid
        "bvid":"BV1se411x7TK", # 视频 bvid
        "view":70346, # 视频播放量
        "danmaku":678, # 视频弹幕数
        "reply":631, # 视频评论数
        "favorite":7911, # 视频收藏数
        "coin":9753, # 视频投币数
        "share":858, # 视频分享量
        "like":12605, # 视频点赞数
        "now_rank":0, # 实时排行
        "his_rank":0, # 历史排行
        "no_reprint":1, # 禁止转载，1：禁止，0：允许
        "copyright":1, # 创作类型，1：自制，2：转载
        "argue_msg":"", # unknown
        "evaluation":"" # unknown
    }
}
~~~

