#作者简介: 
刘亚壮 高级软件架构师 精通大数据与分布式系统架构设计与研发 精通NIO、AIO与Netty开发 精通分布式数据库中间件 国内知名分布式数据库中间件Mycat核心Committer

安装
----
* 确保在你的 AndroidManifest.xml中添加了此项服务
* 在你的class文件中引用此项服务

简单示例
----
```xml
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
         android:versionCode="1"
         android:versionName="1.0">

         <receiver android:name=".MyReceiver" android:enabled="true" android:exported="false">
             <intent-filter>
                 <action android:name="android.intent.action.BOOT_COMPLETED" />
             </intent-filter>
         </receiver>

         <service android:name="com.lyz.mqtt.AMQService" android:exported="false" />

         <uses-permission android:name="android.permission.RECEIVE_BOOT_COMPLETED" />
</manifest>
```


授权声明
-------

    Copyright 2017 liuyazhuang
    
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
    
    http://www.apache.org/licenses/LICENSE-2.0
    
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
