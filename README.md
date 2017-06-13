# LibGDX skins

**LibGDX** comes with a cool *Scene2D* module, which allows you to easily create your GUIs and customize them with `Skin`
instances. However, most beginners struggle with a problem: there is no default skin attached. Not even a simple one.

One could argue that it's the right approach, as it keeps framework's core `jar` smaller - but when you're trying to
learn a new thing, *something* is generally better than *nothing*.

This repository contains *something*.

### [**DOWNLOAD. ALL OF THEM.**](https://github.com/czyzby/gdx-skins/archive/master.zip)

### Free assets

You've probably stumbled upon the [default LibGDX skin](default), which was originally created to test *Scene2D* API in
the official LibGDX repository. It's alright, if you want to test things out - but by the time you're making an actual
LibGDX application, you're probably better off with something less *programmer-art*-ish.

This repository collects free skins contributed by various users at some point. The author thought that it would be
a good idea to keep this kind of stuff in one place - and *not* sharing these assets would be pretty selfish, so this
*one place* turned out to be a public GitHub repository.

So here there are: you're free to check out and use some of the free skins created and uploaded by nice people. Some of
them might be a helpful base for your custom skin, if you don't like starting from scratch. Hell, some can be used as
they are.

Note that the maintainer of this repository does **NOT** plan to track every single skin out there and post updates as
soon as they are available. Most `README` files include links to the sources - if you're interested in a particular
skin, make sure you're using up-to-date assets by yourself. This repository includes skin files for two reasons:
original uploads might expire (or be moved) and it's very convenient to download them all at once to try each one out.

## Additional resources

Using some skin found in the web is one thing, but customizing it - or creating a new one from scratch - is another.
If you're learning *Scene2D* API, make sure to check out these resources.

### Unofficial tools you might not know about

[![LibGDX Texture Packer GUI](.github/images/texture-packer.png)](https://github.com/crashinvaders/gdx-texture-packer-gui)

[Texture Packer GUI](https://github.com/crashinvaders/gdx-texture-packer-gui) allows to create texture atlases from
multiple images. It provides a graphical interface for [the official texture packer tool](https://github.com/libgdx/libgdx/wiki/Texture-packer).

[![IntelliJ LibGDX plugin](.github/images/intellij-plugin.png)](https://github.com/BlueBoxWare/LibGDXPlugin)

[IntelliJ LibGDX plugin](https://github.com/BlueBoxWare/LibGDXPlugin) adds multiple useful LibGDX code inspections and
editors for *Scene2D*-related files (atlases, skins, fonts).

[![VisUI](.github/images/vis-ui.png)](https://github.com/kotcrab/vis-editor/wiki/VisUI)

[VisUI library](https://github.com/kotcrab/vis-editor/wiki/VisUI) extends *Scene2D* with custom widgets and some default
skins. Even if you don't like its default theme (or flat design in general), consider including this library for its
useful new actors.

[![Skin Composer](.github/images/skin-composer.png)](https://github.com/raeleus/skin-composer)

[Skin Composer](https://github.com/raeleus/skin-composer) is a graphical application that allows you to create and edit
custom `Scene2D` skins.

[![gdx-setup](.github/images/gdx-setup.png)](https://github.com/czyzby/gdx-setup)

[Unofficial gdx-setup application](https://github.com/czyzby/gdx-setup) allows to create LibGDX projects. Additionally
to most features provided by the official setup application, it allows to include other JVM languages, more third-party
libraries and use one of predefined project templates.

### Useful links

- [Official Scene2D article](https://github.com/libgdx/libgdx/wiki/Scene2d).
[Scene2D UI](https://github.com/libgdx/libgdx/wiki/Scene2d.ui) and [`Table`](https://github.com/libgdx/libgdx/wiki/Table)
pages are worth your time as well.
- [Official `Skin` article](https://github.com/libgdx/libgdx/wiki/Skin).
- [Official texture packer](https://github.com/libgdx/libgdx/wiki/Texture-packer) and
[Hiero tool](https://github.com/libgdx/libgdx/wiki/Hiero) articles, both of which are useful when preparing `Skin` assets. 
- [Official ninepatches article](https://github.com/libgdx/libgdx/wiki/Ninepatches) might help you understand how to
make skins that look well when resized.
- [KTX library](https://github.com/libktx/ktx) contains [Kotlin](http://kotlinlang.org/) utilities for building
*Scene2D* styles and widgets. It can be a great alternative to error-prone `.json` skin files and overly verbose Java
GUI building code.
- [USL library](https://github.com/kotcrab/vis-editor/wiki/USL) allows you to quickly create *JSON* files thanks to its
simplified, less boilerplate-ish and more powerful syntax. `.usl` files are meant be compiled to LibGDX `.json` skin
definitions before deploying the application - there is no runtime overhead.
- [LML library](https://github.com/czyzby/gdx-lml/tree/master/lml) makes it easier to create your *Scene2D* views.
Instead of verbose Java syntax, LML allows you to create your GUIs with HTML-like templates packed with powerful macros.
With LML, you can separate your GUI layer from application's core logic, and quickly use some easily overlooked LibGDX
features (like *i18n* support) without the usual Java boilerplate. [VisUI](https://github.com/kotcrab/vis-editor/wiki/VisUI)
is also supported in LML thanks to an [extension](https://github.com/czyzby/gdx-lml/tree/master/lml-vis).
- [This article](https://rskupnik.github.io/libgdx-ui-overview) is an amazing introduction into LibGDX GUI tools.
- [GamesFromScratch blog](http://www.gamefromscratch.com/post/2013/11/27/LibGDX-Tutorial-9-Scene2D-Part-1.aspx) includes
a multi-part *Scene2D* tutorial.
- [Pimentoso Software blog](http://pimentoso.blogspot.com/2013/04/libgdx-scene2d-skin-quick-tutorial.html) contains
a simple *Scene2D* tutorial.
- [This thread](http://www.badlogicgames.com/forum/viewtopic.php?f=17&t=22075) contains `TiledNinePatchDrawable`, which
might be necessary for some GUIs.
- Apparently, LibGDX team decided to maintain their own [similar community-driven project](https://github.com/libgdx/libgdx-skins)
 (finally!). It currently contains far less skins, but allows to download them individually and features a live preview.
 If you want to contribute a new skin here, I strongly suggest you also create a pull request to the official
 `libgdx-skins` project. 

### Tools you might have stumbled upon, but should not use

- **Do NOT use [graphical texture packer](https://code.google.com/archive/p/libgdx-texturepacker-gui/)**, unless dealing
with legacy LibGDX version: it is not up-to-date and **can produce corrupt atlases** due to its texture packer version.
You're much better off setting up a Gradle task using the latest `gdx-tools` to pack your atlases (see official texture
packer article for more info how to do this) or using the new [Texture Packer GUI](https://github.com/crashinvaders/gdx-texture-packer-gui).
- [gdx-skineditor](https://github.com/cobolfoo/gdx-skineditor) is a graphical tool that allows to create `Skin` files.
It is not actively maintained, seems to be missing a few features and is known to crash. Use [Skin Composer](https://github.com/raeleus/skin-composer)
instead.
- [This thread](http://www.badlogicgames.com/forum/viewtopic.php?f=17&t=15209) includes *JSON* highlighter for
*IntelliJ/Android Studio* IDEs. Since LibGDX *JSON* parser accepts files with optional quotation (and so on), valid
*Skin* files might appear as corrupted *JSON* files - this highlighter attempts to fix that. However,
[unofficial IntelliJ LibGDX plugin](https://github.com/BlueBoxWare/LibGDXPlugin) addresses this problem and provides
far more additional features, so you might want to use it instead.

## Contributing

Maintainer will gladly accept any pull requests with additional resources - not only new skins, but also useful links
and texts. Helping with keeping skin files up-to-date is also appreciated: don't hesitate to leave an issue or create
a pull request if any resources are outdated.
