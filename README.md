# 号码归属地使用

[![Jdk Version](https://img.shields.io/badge/JDK-1.8-green.svg)](https://img.shields.io/badge/JDK-1.8-green.svg)
[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg)](https://www.apache.org/licenses/LICENSE-2.0.html)
[![Maven Central](https://maven-badges.herokuapp.com/maven-central/link.thingscloud/thingscloud-mobile-area/badge.svg)](https://maven-badges.herokuapp.com/maven-central/link.thingscloud/thingscloud-mobile-area/)

## Maven引入

    <dependency>
        <groupId>link.thingscloud</groupId>
        <artifactId>thingscloud-mobile-area</artifactId>
        <version>1.0.0-RELEASE</version>
    </dependency>


## 使用
    // 获取号码区域 : 区号/省份/地市
    MobileArea.getInstance().getArea("15121001234");
    MobileArea.getInstance().getArea("0015121001234"));
    
    // 获取外呼号码-如果不同区域会自动加 0
    MobileArea.getInstance().getMobileNumber("15121001234", "020");
    MobileArea.getInstance().getMobileNumber("+915121001234", "021");
    
    // 是否是指定区域
    MobileArea.getInstance().isSameArea("915121001234", "020");
    MobileArea.getInstance().isSameArea("9015121007938", "021");

## License

[Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html) Copyright (C) Apache Software Foundation
