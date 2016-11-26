
# Android Proficiency Exercise

## Overview

To verify coding standards and Android knowledge, we ask that the developer who will be performing work for us complete this small test. This proof-of-concept exercise will be evaluated on both the code quality and the final product with equal weighting.

We would like you to create a simple app with the open API provided by [http://gank.io/api](http://gank.io/api). Through this project, you are supposed to show us your
- proficiency on coding skills,
- good comprehension, communication and collaboration skills,
- potential and talents.

## Specification

### API

Read the API documentation of [http://gank.io/api](http://gank.io/api) carefully. You will have to request a json response which lists the posts under these topics `Android`/`iOS`/`前端`.

> GET http://gank.io/api/data/Android/1/1

```json
{
  "error": false,
  "results": [
    {
      "_id": "5833c3b3421aa926e43aef90",
      "createdAt": "2016-11-22T12:04:03.555Z",
      "desc": "随着 Android 引入 Java 8 的一些功能，请记住每一个标准库的 API 和语言特性都会带来一些相关的开销，这很重要。虽然设备越来越快而且内存越来越多，代码大小和性能优化之间仍然是有着紧密关联的。",
      "images": [
        "http://img.gank.io/b530a4e3-9ec8-4166-8c8f-fdd29e11c0d5",
        "http://img.gank.io/8b3cf104-4b27-4dbd-8407-769d622ca077"
      ],
      "publishedAt": "2016-11-23T11:27:52.847Z",
      "source": "web",
      "type": "Android",
      "url": "https://realm.io/cn/news/360andev-jake-wharton-java-hidden-costs-android/",
      "used": true,
      "who": "Chen Mulong"
    }
  ]
}
```

### Product

![Artboard](/materials/Artboard.png)

Take a look on the design work. It's created in Sketch but in case you don't have Sketch installed, png file will also be provided. This app consists of these functions which require you to implement
- a Toolbar with tabs(Android, iOS, 前端), users can switch between these tabs to view posts under a specific topic
- a List to display all kinds of posts
	- pure text
	- text with images(users can swipe to view images)
	- text with GIF(nice to be displayed as GIF, but you may consider it as a jpeg)
- pull down to refresh
- pull up(in the end of the List) to load history(older) posts
- only load the image as needed, make sure users don't have to download the images every time
- click on the item to view detailed information in a WebView
- cache all the posts in database so that you can display data when network is unavailable

#### Sketch Measure

You might need to look up the specific `colors`/`paddings`/`margins`/`font sizes` in [Sketch Measure](/Sketch\ Measure/index.html).

> Tip: Download this project and open `Sketch Measure/index.html` in your browser.

![Sketch Measure](/materials/Sketch-Measure.png)

## Hints

- Communicate with your interviewer when you are confused.
- Use Git to manage the source code and commit as much as you could with a **CLEAR** history.
- Comment your code when you think it's necessary.
- Use clear method and variable names.
- Use Material Design support library and find the icons you need here [https://material.io/icons](https://material.io/icons).
- Feel free to use any third-party library you're familiar with, but choose wisely.
- Try to polish your code as much as possible.
- Impress your interviewer.

## pull request

Once you've finished, you may launch a pull request to this project.

**To make us understand your purpose of pull request, just mark a label on it.**

### Use labels to mark you purpose

- #for-fun
- #for-interview

> Tips: You can find the labels on the right panel in your pull-request/issue editing page. If you don't have the permission then leave a message there and we will set the right label for you.

## Acknowledgements

- [gank.io](http://gank.io)

  [gank.io](http://gank.io) is a platform built by [daimajia](https://github.com/daimajia), famous for it's daily high-quality recommendations. We are truly grateful for using its open API.

- [goeasyway](https://github.com/goeasyway)

  The idea of this kind of interview was stole from a foreign company, first showed up in this blog [post](http://www.jianshu.com/p/3178e527ec76) by [goeasyway](https://github.com/goeasyway).
