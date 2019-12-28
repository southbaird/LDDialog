# LDDialog



[TOC]

## 功能

支持横竖屏自动适配布局

## 效果图

![SM-G9550_20191228105325](C:\Users\Administrator\Desktop\Dialog\LDDialog\image\SM-G9550_20191228105325.gif)

## Gradle 依赖

```
dependencies {
    implementation 'cn.com.blackview:lddialog:1.0.0'
}
```

## 简单使用

```
 				new LDDialog.Builder(MainActivity.this)
                        .setTitle("提示")
                        .setContent("您好，我们将在30分钟处理，稍后通知您订单结果！")
//                        .setCancelableOutSide(true)
                        .setRightButton(new IDialog.OnClickListener() {
                            @Override
                            public void onClick(IDialog dialog) {
                                dialog.dismiss();
                            }
                        })
                        .setLeftButton(new IDialog.OnClickListener() {
                            @Override
                            public void onClick(IDialog dialog) {
                                dialog.dismiss();
                            }
                        })
                        .show();
```

## 更新日志

初始版本