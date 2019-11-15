# mvnrepo
## 用于存放工具包
#### 使用方法
修改Project的**build.gradle**，添加maven地址
```
allprojects {
    repositories {
        google()
        jcenter()
        maven{
            url "https://github.com/LiPengfei0106/mvnrepo/raw/master"
        }
    }
}
```
然后在module中implementation需要的包即可
```
dependencies {
    # 人脸识别库
    implementation 'cn.cleartv.lee:facesdk:0.0.1'
	# 人脸识别库2，和1使用方法基本一样，添加了活体检测等功能
    implementation 'cn.cleartv.lee:facesdk2:0.0.1'
    # Android开发工具库
    implementation 'cn.cleartv.lee:library:0.0.2'
    # Glide support WebP 和 SVG库
    implementation 'cn.cleartv.lee:glide-support:0.0.1'
    # 下载库，通过广播监听下载过程
    implementation 'cn.cleartv.lee:downloader:0.0.1'
    # TV用的部件，包括TvRecyclerView等
    implementation 'cn.cleartv.lee:tvwidget:0.0.1'
    # 身份证读卡器
    implementation 'cn.cleartv.lee:cardreader:0.0.2'
    # 指纹采集
    implementation 'cn.cleartv.lee:fpreader:0.0.1'
    # 中控读取设备，包括读卡器和指纹采集仪
    implementation 'cn.cleartv.lee:zkreader:0.0.8'
    # Rxbus库
    implementation 'cn.cleartv.lee:rxbus:0.0.3'
}
```
