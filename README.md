# 华视电子-台式居民身份证阅读机(CVR-100U)

## 环境

jdk8 32位版本，jnative依赖32位版本的jdk

## 使用方法

* 安装jdk后，将src/resources目录下的.dll文件放入已安装jre的/bin目录下
* 安装阅读器的驱动
* 启动项目，访问/demo/api/test接口，即可获取身份证数据（如果返回身份证数据参数是空，且提示找不到termb.dll文件的话，重启计算机在重启项目即可）

## 坑！！！

如果提示termb.dll找不到异常，请打开cmd 输入where java命令，确保出现的地址一定是与你放入dll文件地址一致。这种情况，通常出现在在安装版本的jdk中，因为安装版jdk会默认使用C:\ProgramData\Oracle\Java下面的命令