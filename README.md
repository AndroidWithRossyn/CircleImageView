[![](https://jitpack.io/v/OmaPrakash/CircleImageView.svg)](https://jitpack.io/#OmaPrakash/CircleImageView)
![GitHub](https://img.shields.io/github/license/OmaPrakash/CircleImageView)

<p align="center">
  <h1 align="center">CircleImageView</h1>
</p>

- ⚡  If You want to join us than message on <a href="banrossyn@gmail.com">Mail</a>
&
<a href="https://t.me/banrossyn">Telegram</a>. 

> Note: `-- Apache License 2.0` you can't Publish any Source code without permission.

# 
<p align="center">
    <a href="https://www.paypal.com/paypalme/banrossyn">
      <img src="https://user-images.githubusercontent.com/97843190/184054819-e2e80e69-df46-4d38-8769-5d591673d412.png" width="300"/>
    </a>
  </p>
<p align="center">If you like my work and Source Code is really helpful for you, <strong>Show Some Love</strong></p>

<p align="center">
    <a >
     <img src="https://user-images.githubusercontent.com/97843190/189529088-cd55a081-3b80-4614-a41b-dd424b70c565.png"/>
    </a>
  </p>

It uses a BitmapShader and does not:

- create a copy of the original bitmap
- use a clipPath (which is neither hardware accelerated nor anti-aliased)
- use setXfermode to clip the bitmap (which means drawing twice to the canvas)

As this is just a custom ImageView and not a custom Drawable or a combination of both, it can be used with all kinds of drawables, i.e. a PicassoDrawable from Picasso or other non-standard drawables (needs some testing though).

### Implemented in these projects
- ![Instagram-Story-Saver](https://github.com/BanRossyn/Instagram-Story-Saver)
- ![InSaver-Reels-Story-Video](https://github.com/BanRossyn/InSaver-Reels-Story-Video)
- ![InStory-Downloader-for-Instagram-Facebook-Whatsapp](https://github.com/BanRossyn/InStory-Downloader-for-Instagram-Facebook-Whatsapp)

## How to:
- gradle

Add the JitPack repository to your build file.
Add this in your root `settings.gradle` file (**not** your module `build.gradle` file):

```gradle

dependencyResolutionManagement {
    repositoriesMode.set(RepositoriesMode.PREFER_SETTINGS)
    repositories {
    ....
        maven { url "https://jitpack.io" }
        ...
    }
}
```

Then, add the library to your module `build.gradle`

```gradle
dependencies {
  implementation 'com.github.OmaPrakash:CircleImageView:(letest Release)'
}
```


```xml
<com.banrossyn.CircleImageView
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:id="@+id/profile_image"
    android:layout_width="96dp"
    android:layout_height="96dp"
    android:src="@drawable/profile"
    app:civ_border_width="2dp"
    app:civ_border_color="#FF000000"/>
```
- maven

```
<repositories>
		<repository>
		    <id>jitpack.io</id>
		    <url>https://jitpack.io</url>
		</repository>
</repositories>

```

```
<dependency>
	    <groupId>com.github.OmaPrakash</groupId>
	    <artifactId>CircleImageView</artifactId>
	    <version>Tag</version>
</dependency>
```



### License
```
Copyright 2022 Rossyn

Licensed to the Apache Software Foundation (ASF) under one or more contributor
license agreements. See the NOTICE file distributed with this work for
additional information regarding copyright ownership. The ASF licenses this
file to you under the Apache License, Version 2.0 (the "License"); you may not
use this file except in compliance with the License. You may obtain a copy of
the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
License for the specific language governing permissions and limitations under
the License.
```
