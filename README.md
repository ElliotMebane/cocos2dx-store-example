*This project is a part of The [SOOMLA](http://www.soom.la) Framework, which is a series of open source initiatives with a joint goal to help mobile game developers do more together. SOOMLA encourages better game design, economy modeling, social engagement, and faster development.*

# cocos2dx-store-example

**cocos2dx-store-example** is an example project demonstrating usage and implementation of SOOMLA's [cocos2dx-store](http://github.com/soomla/cocos2dx-store).

This project contains examples for implementing all of SOOMLA's interfaces and using SOOMLA's various services. Read up on what you can do with SOOMLA in this [wiki](https://github.com/soomla/android-store/wiki) (the wiki is for Android but it applies to all the projects under The SOOMLA Project).

## Getting started

While the 3rd version of cocos2d-x is not stable, we put all related code to branch: `cocos2dx-v3`. Please, consider to check out to this branch in example project, and in cocos2dx-store.

1. Obtain the Cocos2d-x framework either from [git](https://github.com/cocos2d/cocos2d-x) or from the [Cocos2d-x website](http://www.cocos2d-x.org/download). Make sure to use the latest stable 3rd version of cocos2d-x (we tested with v3.0rc1).
    ```
    $ git clone git@github.com:cocos2d/cocos2d-x.git
    ```

2. Clone [soomla-cocos2dx-core](https://github.com/soomla/soomla-cocos2dx-core) and [cocos2dx-store](https://github.com/soomla/cocos2dx-store) into the `extensions` directory in the root of your Cocos2d-x framework.
    ```
    $ cd cocos2dx
    $ git clone git@github.com:soomla/soomla-cocos2dx-core.git extensions/soomla-cocos2dx-core
    $ git clone git@github.com:soomla/cocos2dx-store.git extensions/cocos2dx-store
    ```

3. Clone our [fork](https://github.com/vedi/jansson) of the janssen library into the `external` directory in the root of your Cocos2d-x framework.
    ```
    $ git clone git@github.com:vedi/jansson.git external/jansson
    ```

4. Clone cocos2dx-store-example into the `projects` directory at the root of the Cocos2d-x framework.
    ```
    $ git clone git@github.com:soomla/cocos2dx-store-example.git projects/cocos2dx-store-example
    ```

Note: Draw your attention, we use symlink to cocos2d-x in our example project. It relies on cocos2d-x availability in relative path. If you want to use the project from other location, update the symlink, or completely replace it with cocos2d-x folder.

#### Build instructions for Android

1. Run the `build_native.sh` script located in projects/cocos2dx-store-example/proj.android. This step should take a while.
    ```
    $ cd projects/cocos2dx-store-example/proj.android
    $ ./build_native.py
    ```

2. Finally, open the `proj.android` directory located in `cocos2dx-store-example` in Android Studio (IntelliJ IDEA). `proj.android` is an Android Studio project.
3. Build the project, run example activity, and you're ready to go! The application should launch in an emulator or on your device.

Take a look around, and get a feel for all you can do with cocos2dx-store.


#### Build instructions for iOS

1. Open the XCode project under `proj.ios_mac`.
2. Build the project, run it, and you're ready to go! The application should launch in the simulator or on your device.

Take a look around, and get a feel for all you can do with cocos2dx-store.

#### CCIStoreAssets

A good example of how to define an economy model can be found in [MuffinRushAssets](https://github.com/soomla/cocos2dx-store-example/blob/master/Classes/MuffinRushAssets.cpp).

Take a look at that file and see how you can define your specific game's economy.

#### Scenes

This project contains three main scenes: MainScene, StoreAScene, and StoreBScene. They are all built with [*CocosBuilder*](http://cocosbuilder.com/)
- **MainScene**: serves as an entry point to the store, use it as a reference how to enter the store in your app.
- **StoreAScene**: contains all of the PurchaseWithVirtualItem items and allows the user to buy them.
- **StoreBScene**: contains all of the PurchaseWithMarket items and allows the user to buy them.

Contribution
---
SOOMLA appreciates code contributions! You are more than welcome to extend the capabilities of SOOMLA.

Fork -> Clone -> Implement -> Add documentation -> Test -> Pull-Request.

IMPORTANT: If you would like to contribute, please follow our [Documentation Guidelines](https://github.com/soomla/cocos2dx-store/blob/master/documentation.md
). Clear, consistent comments will make our code easy to understand.

## SOOMLA, Elsewhere ...

+ [Framework Website](http://www.soom.la/)
+ [Knowledge Base](http://know.soom.la/)


<a href="https://www.facebook.com/pages/The-SOOMLA-Project/389643294427376"><img src="http://know.soom.la/img/tutorial_img/social/Facebook.png"></a><a href="https://twitter.com/Soomla"><img src="http://know.soom.la/img/tutorial_img/social/Twitter.png"></a><a href="https://plus.google.com/+SoomLa/posts"><img src="http://know.soom.la/img/tutorial_img/social/GoogleP.png"></a><a href ="https://www.youtube.com/channel/UCR1-D9GdSRRLD0fiEDkpeyg"><img src="http://know.soom.la/img/tutorial_img/social/Youtube.png"></a>

## License

Apache License. Copyright (c) 2012-2014 SOOMLA. http://soom.la
+ http://opensource.org/licenses/Apache-2.0

