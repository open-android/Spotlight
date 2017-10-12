# Spotlight

### 一分钟实现引导界面

* 在github上面看到一个不错的国外开源项目，主要实现欢迎或者引导界面，为了方便大家学习，本人把英文版本的开源项目翻译成中文版本，并且代码已经运行而且运用到项目当中，实测问题不大，如果各位感觉这样的行为比较挫，或者比较鄙视这种行为可以参考原文英文版本，英文版本链接如下：

* 英文 原链接如下：https://github.com/wooplr/Spotlight




# Screen

<img src="https://raw.githubusercontent.com/wooplr/Spotlight/master/art/intro.gif?token=AA5ZAHdvAspW6Zj8YyyKamkV7jWXFtMHks5XaQovwA%3D%3D"/>

### 把如下代码拷贝到JAVA代码中：

```java
new SpotlightView.Builder(this)
        .introAnimationDuration(400)
        .enableRevealAnimation(isRevealEnabled)
        .performClick(true)
        .fadeinTextDuration(400)
        .headingTvColor(Color.parseColor("#eb273f"))
        .headingTvSize(32)
        .headingTvText("Love")
        .subHeadingTvColor(Color.parseColor("#ffffff"))
        .subHeadingTvSize(16)
        .subHeadingTvText("Like the picture?\nLet others know.")
        .maskColor(Color.parseColor("#dc000000"))
        .target(view)
        .lineAnimDuration(400)
        .lineAndArcColor(Color.parseColor("#eb273f"))
        .dismissOnTouch(true)
        .dismissOnBackPress(true)
        .enableDismissAfterShown(true)
        .usageId(usageId) //UNIQUE ID
        .show();
```

## Download
### Gradle

1. Define the jitpack remote Maven repository inside the repositories block of your root `build.gradle` file

    ```javascript
    allprojects {
        repositories {
            ...
            maven { url "https://jitpack.io" }
        }
    }
    ```

2. Add the Spotlight dependency

    ```javascript
    dependencies {
        ...
        compile 'com.github.wooplr:Spotlight:1.2.3'
    }
    ```

