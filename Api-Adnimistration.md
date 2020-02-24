## 0.1 图片上传  
URL:/image/upload  
method:Post  
Requst Context-type:multipart

ResponsBoty:  
"'  
http://xxx.com/xxx1.jpg
'"

Request Field  
| 字段 | 类型 | 描述 |  
| image | String | 文件上传 |  
  
Respone Filed  
| 字段 | 类型 | 描述 |  
|  | String | 上传文件后Url |  
## 1.1 管理员登陆  
URL: /administrator/login?jusername={username}&password={password}   
method: GET  

ResponseBoby:  
"'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c'"  


Request Field    
| 字段 | 类型 | 描述 |  
| username | String | 用户名 |  
| password | String | 密码 |  
    
Response File  
| 字段 | 类型 | 描述 |  
| | String | jwt token |  
## 1.2 管理员获取Profile  
URL: /administrator/getProfile   
method: GET  

ResponseBoby:  
"'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c'"  

ResponseBoty  
"'json  
{
    "administratorId":"1234"  
    "username":"cxy"  
    "realName":"嘻嘻"  
    "email":"123456789@qq.com"  
    "status":"1"  
    "createTime":123456  
    "avatarUrl":"xxx.jpg"  
}  
'"  
Requset Header  
| 字段 | 类型 | 描述 |  
| :-------: | :-------: | :-------: |  
| jcartToken | String | jwt token |  
Response File  
| 字段 | 类型 | 描述 |  
| administratorId | int | 管理员id |  
| username | String | 用户名称 |  
| realName | String | 真实名 |  
| email | String | 邮箱 |  
| status | byte | 状态 |  
| createTime | Long | 创建时间 |  
| avatarUrl | String | 头像地址 |  
## 1.3 管理员更新Profile
URL: /administrator/UpdateProfile   
method: POST  

ResponseBoby:  
"'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c'"  

RequestBody:  
"'json  
{
    "password":"123"  
    "realNmae":"嘻嘻"  
    "email":"123456.qq.com"  
    "avatarUrl":"xxx1.jpg"  
    "status":1  
}
'"  
Requset Header  
| 字段 | 类型 | 描述 |  
| :-------: | :-------: | :-------: |  
| jcartToken | String | jwt token |  

Response File  
| 字段 | 类型 | 描述 |  
| password | String | 密码 |  
| realNmae | String | 真实名称 |  
| email | String | :-------: |   
| avatarUrl | String | 头像地址 |  
| status | Byte | 状态 |  
## 1.4 管理员获取密码重置码

## 1.5 管理员重置密码

## 1.6 管理员搜索列表

## 1.7 管理员回显

## 1.8 管理员创建

## 1.9 管理员更新