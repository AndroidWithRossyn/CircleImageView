

<p align="center">
  <h1 align="center">CircleImageView</h1>
</p>

<div align="center">
	
[![](https://jitpack.io/v/OmaPrakash/CircleImageView.svg)](https://jitpack.io/#OmaPrakash/CircleImageView)
![GitHub](https://img.shields.io/github/license/OmaPrakash/CircleImageView)
<a href="https://t.me/banrossyn" target="_blank"><img src="https://img.shields.io/badge/Telegram-%40banrossyn-28a8ea"></a>
<a href="https://wa.me/+919694260426/" target="_blank"><img src="https://img.shields.io/badge/whatsapp-%40+919694260426-28a8ea"></a>
<a href="https://www.linkedin.com/in/banrossyn/" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-banrossyn-informational"></a>
<a href="mailto:banrossyn@gmail.com"><img src="https://img.shields.io/badge/Email-banrossyn%40gmail.com-blue"></a>

</div>

# 


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




