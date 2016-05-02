#build.gradle文件配置

###project下的build.gradle文件

```java
   classpath 'com.jfrog.bintray.gradle:gradle-bintray-plugin:1.6'
   classpath 'com.github.dcendents:android-maven-gradle-plugin:1.3'
```

###module下的build.gradle文件

```java
ext {
    bintrayRepo = 'maven'     //bintray上的仓库名，一般为maven
    bintrayName = 'RestHttp'   //bintray上的项目名

    publishedGroupId = 'cn.alien95'    //jcenter的GroupId：一般是包名
    artifact = 'resthttp'     //jcenter的ArtifactId：一般是项目名
    libraryVersion = '1.0.1-beta1'    //发布的版本号：每次上传必须不一样

    siteUrl = 'https://github.com/llxdaxia/RestHttp'       //网站地址
    gitUrl = 'https://github.com/llxdaxia/RestHttp.git'    //git地址

    libraryName = 'RestHttp'       //项目名字
    libraryDescription = 'A network framework for Android'     //项目描述

    //开发者信息
    developerId = 'Lemon'
    developerName = 'Lemon'
    developerEmail = 'daxiallx@gmail.com'

    //以上所有信息自行修改，以下不变
    licenseName = 'The Apache Software License, Version 2.0'
    licenseUrl = 'http://www.apache.org/licenses/LICENSE-2.0.txt'
    allLicenses = ["Apache-2.0"]
}
apply from: 'https://raw.githubusercontent.com/llxdaxia/GradleScript/master/bintray_v1.gradle'
apply from: 'https://raw.githubusercontent.com/llxdaxia/GradleScript/master/bintray_v1.gradle'

//或者以下版本
//apply from: 'https://raw.githubusercontent.com/llxdaxia/GradleScript/master/install.gradle'
//apply from: 'https://raw.githubusercontent.com/llxdaxia/GradleScript/master/bintray.gradle'
```

