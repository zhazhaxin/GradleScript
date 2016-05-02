#build.gradle文件配置

```java
ext {
    bintrayRepo = 'maven'////bintray上的仓库名，一般为maven
    bintrayName = 'RestHttp'//bintray上的项目名

    publishedGroupId = 'cn.alien95'//JCenter的GroupId
    artifact = 'resthttp'//JCenter的ArtifactId
    libraryVersion = '1.0.1-beta1'//版本号

    siteUrl = 'https://github.com/llxdaxia/RestHttp'
    gitUrl = 'https://github.com/llxdaxia/RestHttp.git'

    libraryName = 'RestHttp'//项目名字，没什么用
    libraryDescription = 'A network framework for Android'//项目描述，没什么用

    //开发者信息
    developerId = 'Lemon'
    developerName = 'Lemon'
    developerEmail = 'daxiallx@gmail.com'

    //以上所有信息自行修改，以下不变

    licenseName = 'The Apache Software License, Version 2.0'
    licenseUrl = 'http://www.apache.org/licenses/LICENSE-2.0.txt'
    allLicenses = ["Apache-2.0"]
}
apply from: 'https://raw.githubusercontent.com/llxdaxia/GradleScript/master/install.gradle'
apply from: 'https://raw.githubusercontent.com/llxdaxia/GradleScript/master/bintray.gradle'
```

