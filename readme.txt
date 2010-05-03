=== Cover Flow FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, cover, flow, coverflow, itunes, free, flash, page, slide, portfolio, book, flip, gallery, slideshow, auto, scroll, rotator, scroller, tooltip, text, 3d, scrollbar, image, effect, preloader, as3, horizontal, photo, images, photos, widget, post, plugin, posts, sidebar
Requires at least: 2.8.0
Tested up to: 2.9.2
Stable tag: trunk

== Description ==

One of the most advanced Cover Flows on the web. Completely XML customizable, without using Flash.

= Main features =

The Cover Flow FX can be embedded in any website for free without even using Flash and it can have an overall width and height up to 1680 x 1050 pixels.
The Cover Flow uses the Papervision3D engine and has multiple plane and camera views. It supports all types of images (JPG, GIF, BMP, PNG) which can have different sizes - they will be automatically adjusted to fit in the same height. It has an auto play function with external PNGs (customizable) for play/pause buttons. Optional scroll bar with multiple skins to choose from. Extensive configurations for tooltip and reflection.

== Installation ==

Make sure your Wordpress version is equal or greater than 2.8 and your hosting provider is using PHP5.

1. Upload the `cover-flow-fx` directory along with all its files to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. In the post editor use the following tag to embed the Cover Flow: `[cover-flow-fx][/cover-flow-fx]`. Or add `<?php coverflowfx_echo_embed_code(); ?>` in your templates
4. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Cover Flow](http://www.flashxml.net/cover-flow.html "Cover Flow") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `component/settings.xml`
5. To use your own images, upload them to the `component/images` directory and update the `component/images.xml` file accordingly

= No Flash support text =

To support visitors without Adobe Flash, you can provide alternative textual content. From the post editor, add the text between `[cover-flow-fx]` and `[/cover-flow-fx]`. From the PHP files of your theme, add the text as *the first argument* of the `coverflowfx_echo_embed_code()` function call.

= Additional settings file =

To embed the Cover Flow more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called **settings2.xml**. From the post editor, use the following code: `[cover-flow-fx settings="settings2.xml"][/cover-flow-fx]`. From the PHP files of your theme, add the file name as *the second argument* of the `coverflowfx_echo_embed_code()` function call. If you use a separate set of images, don't forget to create a new XML file for that and update the `imagesXML` value in the settings file.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/cover-flow.html "Cover Flow") is the utility that helps easily customize your Cover Flow to fit all of your needs.