# *- 安卓用户企鹅阅读 Cookies修改指南 -*

## 感谢sazs34大佬的替换思路和脚本  https://github.com/sazs34  
## 感谢ZIYE制作的企鹅阅读脚本  https://github.com/18u  
## 感谢telegram群的Money Mr提供脚本 https://t.me/qhqcz
## 感谢Addr大佬指导的安卓抓包教程 https://github.com/paopaoya

### 安卓用户抓包Secrets格式如下所示  
{"ywsession":"填写你的ywsession信息","Cookie":"填写你QQREADHEADERKEY的cookie","Connection":"keep-alive","Content-Type":"application/json","Accept":"\*/\*\","Host":"mqqapi.reader.qq.com","User-Agent":"你抓到的UserAgent","Referer":"Referer链接","Accept-Language":"zh-cn","Accept-Encoding":"gzip, deflate, br","mpversion":"这个安卓和IOS的不一致，自己填"}@填写你的QQReadtimeurlVal@{"ywsession":"填写你的ywsession信息","Cookie":"填写你QQREADHEADERKEY的cookie,长一点的，带openid的","Connection":"keep-alive","Content-Type":"application/json","Accept":"\*/\*\","Host":"mqqapi.reader.qq.com","User-Agent":"你抓到的UserAgent","Referer":"Referer链接","Accept-Language":"zh-cn","Accept-Encoding":"gzip, deflate, br","mpversion":"这个安卓和IOS的不一致，自己填"}





#### 样例：  
{"ywsession":"ywn","Cookie":"ck1","Connection":"keep-alive","Content-Type":"application/json","Accept":"*/*","Host":"mqqapi.reader.qq.com","User-Agent":"UA","Referer":"https://appservice.qq.com/1110657249/0.30.0/page-frame.html","Accept-Language":"zh-cn","Accept-Encoding":"gzip, deflate, br","mpversion":"0.30.0"}@qqreadtimeurlVal@{"ywsession":"ywn","Cookie":"ck2","Connection":"keep-alive","Content-Type":"application/json","Accept":"*/*","Host":"mqqapi.reader.qq.com","User-Agent":"UA","Referer":"https://appservice.qq.com/1110657249/0.30.0/page-frame.html","Accept-Language":"zh-cn","Accept-Encoding":"gzip, deflate, br","mpversion":"0.30.0"}

ywsession=ywn

qqreadheaderVal cookie=ck1

User-Agent=UA

qqreadtimeurlVal=qqreadtimeurlVal

qqreadtimeheaderVal cookie=ck2

替换即可
### 多账号格式,直接换行就行  
账号1的qqreadheaderVal@qqreadtimeurlVal@qqreadtimeheaderVal  
账号2的qqreadheaderVal@qqreadtimeurlVal@qqreadtimeheaderVal  
账号3的qqreadheaderVal@qqreadtimeurlVal@qqreadtimeheaderVal  

### 安卓抓包工具  
HttpCanary（我用的）

qqreadurlVal https://mqqapi.reader.qq.com/mqq/user/init

qqreadheaderVal   ck1

qqreadtimeurlVal     ReadTimeWithBid

qqreadtimeheaderVal    ck2
