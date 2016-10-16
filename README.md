# LibGDX skins

**LibGDX** comes with a cool *Scene2D* module, which allows you to easily create your GUIs and customize them with `Skin` instances. However, most beginners struggle with a problem: there is no default skin attached. Not even a simple one.

One could argue that it's the right approach, as it keeps framework's core `jar` smaller - but when you're trying to learn a new thing, *something* is generally better than *nothing*.

This repository contains *something*. (Actually, a few somethings.)

#### [**DOWNLOAD. ALL OF THEM.**](https://github.com/czyzby/gdx-skins/archive/master.zip)

### Free assets

You've probably stumbled upon the [default LibGDX skin](default), which was originally created to test *Scene2D* API in the official LibGDX repository. It's alright, if you want to test things out - but by the time you're making an actual LibGDX application, you're probably better off with something less *programmer-art*-ish.

This repository collects free skins contributed by various users at some point. The author thought that it would be a good idea to keep this kind of stuff in one place - and *not* sharing these assets would be pretty selfish, so this *one place* turned out to be a public GitHub repository.

So here there are: you're free to check out and use some of the free skins created and uploaded by nice people. Some of them might be a helpful base for your custom skin, if you don't like starting from scratch. Hell, most can be used as they are.

Note that the maintainer of this repository does **NOT** plan to track every single skin out there and post updates as soon as they are available. Most `README` files include links to the sources - if you're interested in a particular skin, make sure you're using up-to-date assets by yourself. This repository includes skin files for two reasons: original uploads might expire (or be moved) and it's very convenient to download them all at once to try each one out.

### Additional resources

Using some skin found in the web is one thing, but customizing it - or creating a new one from scratch - is another. If you're learning *Scene2D* API, make sure to go through these links:

- [Official Scene2D article](https://github.com/libgdx/libgdx/wiki/Scene2d). [Scene2D UI](https://github.com/libgdx/libgdx/wiki/Scene2d.ui) and [`Table`](https://github.com/libgdx/libgdx/wiki/Table) pages are worth your time as well.
- [Official `Skin` article](https://github.com/libgdx/libgdx/wiki/Skin).
- [Official texture packer](https://github.com/libgdx/libgdx/wiki/Texture-packer) and [Hiero tool](https://github.com/libgdx/libgdx/wiki/Hiero) articles, both of which are useful when preparing `Skin` assets. **Do NOT use [graphical texture packer](https://code.google.com/archive/p/libgdx-texturepacker-gui/)**, unless dealing with legacy LibGDX version: it doesn't seem to be up-to-date and **can produce corrupt atlases**. You're much better off setting up a Gradle task using the latest `gdx-tools` to pack your atlases (see official texture packer article for more info how to do this).
- [Official ninepatches article](https://github.com/libgdx/libgdx/wiki/Ninepatches) might help you understand how to make skins that look well when resized.
- [Skin Composer](https://github.com/raeleus/skin-composer) is a graphical application that allows you to create and edit custom `Scene2D` skins. Created by [Raeleus](https://ray3k.wordpress.com/software/skin-composer-for-libgdx/).
- [gdx-skineditor](https://github.com/cobolfoo/gdx-skineditor) is an application that allows you to create custom skins. While it doesn't seem to be currently maintained (and is able to crash from time to time), it might still prove useful. Keep in mind that it's still worth to understand skin's *JSON* internals before using this tool.
- [VisUI library](https://github.com/kotcrab/vis-editor/wiki/VisUI) extends *Scene2D* with custom widgets and some default skins. Even if you don't like its flat design theme, consider including this library for its new useful actors.
- [USL library](https://github.com/kotcrab/vis-editor/wiki/USL) allows you to quickly create *JSON* files thanks to its simplified, less boilerplate-ish and more powerful syntax. `.usl` files are meant be compiled to LibGDX `.json` skin definitions before deploying the application - there is no runtime overhead.
- [KTX library](https://github.com/czyzby/ktx) contains [Kotlin](http://kotlinlang.org/) utilities for defining *Scene2D* styles and widgets. It can be a great alternative to error-prone `.json` skin files and overly verbose Java GUI building code.
- [LML library](https://github.com/czyzby/gdx-lml/tree/master/lml) makes it easier to create your *Scene2D* views. Instead of verbose Java syntax, LML allows you to create your GUIs with HTML-like templates packed with powerful macros. With LML, you can separate your GUI layer from application's core logic, and quickly use some easily overlooked LibGDX features (like *i18n* support) without the usual Java boilerplate. [VisUI](https://github.com/kotcrab/vis-editor/wiki/VisUI) is also supported in LML thanks to an [extension](https://github.com/czyzby/gdx-lml/tree/master/lml-vis).
- [GamesFromScratch blog](http://www.gamefromscratch.com/post/2013/11/27/LibGDX-Tutorial-9-Scene2D-Part-1.aspx) includes a multi-part *Scene2D* tutorial.
- [Pimentoso Software blog](http://pimentoso.blogspot.com/2013/04/libgdx-scene2d-skin-quick-tutorial.html) contains a simple *Scene2D* tutorial.
- [This thread](http://www.badlogicgames.com/forum/viewtopic.php?f=17&t=15209) includes *JSON* highlighter for *IntelliJ/Android Studio* IDEs. No more red spots in your skin files!
- [This thread](http://www.badlogicgames.com/forum/viewtopic.php?f=17&t=22075) contains `TiledNinePatchDrawable`, which might be necessary for some GUIs.
- Apparently, LibGDX team decided to maintain their own [similar community-driven project](https://github.com/libgdx/libgdx-skins) (finally!). It currently contains far less skins, but allows to download them individually and features a live preview. If you want to contribute a new skin here, I strongly suggest you also create a pull request to the official `libgdx-skins` project. 

## Contributing

Maintainer will gladly accept any pull requests with additional resources - not only new skins, but also useful links and texts. He'd appreciate help with keeping skin files up-to-date: if this repository helped you with your application, the least you could do is check if any resources require an update and leave an issue or create a pull request.
