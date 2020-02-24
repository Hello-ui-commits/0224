## 1.1 客户注册
URL:/customer/register  
method: Post
RequestBoty:
"'json  
{
    "usernmae":"test01"  
    "realName":"张三"  
    "mobile":"120"  
    "email":"1875615710@qq.com"  
    "password":"123456"  
    "nwesSubscribed":false  
}
'"  
ResponseBoty:  
"'  
    123456
'"  
Requset File  
| 字段 | 类型 | 描述 |  
| usernmae | int | 管理员id |  
| realName | String | 用户名称 |  
| mobile | String | 真实名 |  
| email | String | 邮箱 |  
| password | String | 密码 |  
| nwesSubscribed | Boolean | 创建时间 |  
Response Filed  
| 字段 | 类型 | 描述 |  
| :-------: | :-------: | :-------: |  
|  | Integer | 客户Id |  
## 1.2 客户登陆
URL:/customer/login?username={username}&password={password}  
method: Get  

ResponseBoty:
"'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c'"  

Requset File  
| 字段 | 类型 | 描述 |  
| username | String | 用户名 |  
| password | String | 密码 |  

Response File
| 字段 | 类型 | 描述 |  
|  | String | jwt token |  
## 1.3 客户修改密码
RUL:/customer/changePassword  
method: POST  

RequstHeader:
jwtToken:xxx

RequestBody:
"'json  
{
  "originPwd":"123456"  
  "newPwd":"123"  
}
'"  
Request Field  
| 字段 | 类型 | 描述 |  
| jwtToken | String | 登录成功后的jwt |  

Response Filed  
| 字段 | 类型 | 描述 |  
| originpwd | String | 用户名 |  
| newPwd | String | 真实姓名 |
  