# 日期分析节假日分析工作日分析

#### 介绍

 **接口地址：** 
[http://zctool.xyz/public/dateAnalysis](http://zctool.xyz/public/dateAnalysis)

 **请求方式：** GET、POST

 **请求参数：** date（yyyy-MM-dd格式），不传默认当天

 **返回结果：** 
- code：请求状态码（0成功，非0错误）
- message：操作信息
- data：日期结果

- data.date：日期（yyyy-MM-dd格式）
- data.dt：日期类型（平日，补班，放假）
- data.dow：周几（1-7）
- data.ft：节日类型（无，元旦，春节，清明，劳动节，端午节，中秋节，国庆节）
- data.wtw：是否工作日（工作日，休息日）

 **请求例子：** 
GET [http://zctool.xyz/public/dateAnalysis?date=2022-01-01](http://zctool.xyz/public/dateAnalysis?date=2022-01-01)
```json
{
  "message": "操作成功",
  "code": 0,
  "data": {
    "dt": "放假",
    "date": "2022-01-01",
    "wtw": "休息日",
    "dow": "6",
    "ft": "元旦"
  }
}
```
 **请求频率：** 单IP一天10000次

作者联系QQ：137357621

捐赠作者提升服务器性能，提高访问次数
![输入图片说明](WechatIMG201.jpeg)
