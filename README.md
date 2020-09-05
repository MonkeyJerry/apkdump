# apkdump

## 前提

node环境

```
node -v
```

> node环境管理可参考我的博客https://1eq066.coding-pages.com/post/nvm/



## 解析androidmanifest.xml

```
node apkdump.js <apk包>
```

输出解析后json数据到指定文件

```
node apkdump.js <apk包> > apk.json
```



## 解析示例

```
node apkdump.js TikTok_9.8.3.apk > apk.json
```

```
{
    "versionCode": 983,
    "versionName": "9.8.3",
    "installLocation": 0,
    "compileSdkVersion": 28,
    "compileSdkVersionCodename": "9",
    "package": "com.ss.android.ugc.trill",
    "platformBuildVersionCode": 983,
    "platformBuildVersionName": "9.8.3",
    "usesPermissions": [
        {
            "name": "android.permission.ACCESS_FINE_LOCATION"
        },
        {
            "name": "android.permission.ACCESS_COARSE_LOCATION"
        },
        {
            "name": "android.permission.INTERNET"
        },
        {
            "name": "android.permission.INTERNET"
        },
        ...
```

