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
    # Android开发工具库
    implementation 'cn.cleartv.lee:library:0.0.1'
    # Glide support WebP 和 SVG库
    implementation 'cn.cleartv.lee:glide-support:0.0.1'
}
```
