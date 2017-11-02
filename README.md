# ForegroundView

[![Platform](http://img.shields.io/badge/platform-android-brightgreen.svg?style=flat)](http://developer.android.com/index.html)
[![API](https://img.shields.io/badge/API-14%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=14)
[![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Download](https://jitpack.io/v/mutahirqureshi/ForegroundView.svg)](https://jitpack.io/#mutahirqureshi/ForegroundView)

A collection of Android foreground-enabled views just like FrameLayout. Support following views and viewgroups
* ForegroundImageView
* ForegroundButton
* ForegroundTextView
* ForegroundImageButton
* ForegroundEditText
* ForegroundWebView
* ForegroundLinearLayout
* ForegroundRelativeLayout
* ForegroundGridLayout
* ForegroundGridView
* ForegroundHorizontalScrollView
* ForegroundListView
* ForegroundScrollView

# Screenshots
![GitHub Logo](https://lh6.googleusercontent.com/-afY-VQnVodw/Vga8AjKwFkI/AAAAAAAAMko/RtCMUSkNsqY/w487-h865-no/Screenshot_20150926-223701.png)

# Setup

##### Gradle (JitPack)

In your root build.gradle:
```groovy
allprojects {
    repositories {
        jcenter()
        maven { url "https://jitpack.io" }
    }
}
```

In your project build.gradle:
```groovy
dependencies {
    compile 'com.github.mutahirqureshi:foregroundview:{latest_release_version}'
}
```

# Usages

Add Foregroundxxx to your layout.xml

```
        <com.mutahirqureshi.foreground.widget.ForegroundLinearLayout
            android:layout_width="match_parent"
            android:layout_height="64dp"
            android:foreground="@drawable/foreground">
            //child views
        </com.mutahirqureshi.foreground.widget.ForegroundLinearLayout>
```
Foreground view supports 3 additional attributes that you can define in layout file

* android:foreground
* foregroundInsidePadding
* android:foregroundGravity

Alternatively, you can use Java method to change foreground attributes at runtime:
* setForeground(Drawable)
* setForegroundGravity(int)

Checkout sample app to see more details

# Credits

This project has been forked from [ForegroundView](https://github.com/baole/ForegroundView) library by Bao Le Duc, which is licensed under the Apache License, Version 2.0.

# License

	Copyright 2017 Muhammad Qureshi

	Licensed under the Apache License, Version 2.0 (the "License");
	you may not use this file except in compliance with the License.
	You may obtain a copy of the License at

	    http://www.apache.org/licenses/LICENSE-2.0

	Unless required by applicable law or agreed to in writing, software
	distributed under the License is distributed on an "AS IS" BASIS,
	WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
	See the License for the specific language governing permissions and
	limitations under the License.
