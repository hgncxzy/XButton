### 简介

收集了 Android 常用的按钮样式，使用自定义 style 和结合 shape 属性的方式来实现。主要包含了如下按钮：

1. 自定义宽高的实心按钮
2. 固定宽高的实心按钮
3. 自定义宽高的线框按钮
4. 固定宽高的线框按钮
5. 圆角按钮
6. 可以设置圆角、渐变、间隔、大小、填充、描边的按钮

### 展示效果

![效果演示](https://github.com/hgncxzy/XButton/blob/master/gif/GIF.gif)

### 实现方式 1

1. 定义 style 样式
2. 给按钮添加 style 属性

### 实现方式 2

1. 定义 drawable 背景资源
2. 给按钮添加 background 属性

### Shape 属性

```xml
<?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android" >

    <!-- 圆角 -->
    <corners
        android:radius="9dp"
        android:topLeftRadius="12dp"
        android:topRightRadius="12dp"
        android:bottomLeftRadius="12dp"
        android:bottomRightRadius="12dp"/><!-- 设置圆角半径 -->

    <!-- 渐变 -->
    <gradient
        android:startColor="@android:color/white"
        android:centerColor="@android:color/black"
        android:endColor="@android:color/black"
        android:useLevel="true"
        android:angle="45"
        android:type="radial"
        android:centerX="0"
        android:centerY="0"
        android:gradientRadius="90"/>

    <!-- 间隔 -->
    <padding
        android:left="2dp"
        android:top="2dp"
        android:right="2dp"
        android:bottom="2dp"/><!-- 各方向的间隔 -->

    <!-- 大小 -->
    <size
        android:width="250dp"
        android:height="50dp"/><!-- 宽度和高度 -->

    <!-- 填充 -->
    <solid
        android:color="@android:color/holo_purple"/><!-- 填充的颜色 -->

    <!-- 描边 -->
    <stroke
        android:width="2dp"
        android:color="@android:color/black"
        android:dashWidth="1dp"
        android:dashGap="2dp"/>

</shape>

```

### 作者

1. ID : hgncxzy
2. 邮箱：[hgncxzy@qq.com](mailto:hgncxzy@qq.com)
3. 项目地址：https://github.com/hgncxzy/XButton