=== Cover Flow FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, cover, flow, coverflow, itunes, free, flash, page, slide, portfolio, book, flip, gallery, slideshow, auto, scroll, rotator, scroller, tooltip, text, 3d, scrollbar, image, effect, preloader, as3, horizontal, photo, images, photos, widget, post, plugin, posts, sidebar
Requires at least: 2.8.0
Tested up to: 3.0
Stable tag: trunk

== Description ==

One of the most advanced Cover Flows on the web. Completely XML customizable, without using Flash.

= Main features =

The Cover Flow FX can be embedded in any website for free without even using Flash and it can have an overall width and height up to 1680 x 1050 pixels. I uses the Papervision3D engine and has multiple plane and camera views. It supports all types of images (JPG, GIF, BMP, PNG) which can have different sizes - they will be automatically adjusted to fit in the same height. It has an auto play function with external PNGs (customizable) for play/pause buttons. Optional scroll bar with multiple skins to choose from. Extensive configurations for tooltip and reflection.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. [Download](http://www.flashxml.net/free/download/cover-flow.zip "Cover Flow FX") or [purchase](http://www.flashxml.net/cover-flow.html#swmi-license "Cover Flow FX") the Cover Flow FX Flash component
2. Create a new folder inside your `/wp-content/` directory called `flashxml/cover-flow-fx` and copy the content of the archive to this folder
3. Install [the plugin](http://downloads.wordpress.org/plugin/cover-flow-fx.zip "Cover Flow FX Plugin") or upload the `cover-flow-fx` folder along with all its files to `/wp-content/plugins/` directory
4. Activate the plugin from the **Plugins** tab in **WordPress Dashboard**
5. Go to **Cover Flow FX** from the **Settings** tab and update the path in case you used a different one
6. In the post editor use the following tag to embed the Cover Flow FX: `[cover-flow-fx][/cover-flow-fx]`. You could also add `<?php coverflowfx_echo_embed_code(); ?>` in the PHP file of your theme
7. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Cover Flow FX](http://www.flashxml.net/cover-flow.html "Cover Flow FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `flashxml/cover-flow-fx/settings.xml`
8. To use your own images, upload them to the `flashxml/cover-flow-fx/images` folder and update the `flashxml/cover-flow-fx/images.xml` file accordingly

= Additional settings file =

To embed the Cover Flow FX more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called **settings2.xml**. From the post editor, use the following code: `[cover-flow-fx settings="settings2.xml"][/cover-flow-fx]`. From the PHP files of your theme, add the file name as *the first argument* of the `coverflowfx_echo_embed_code()` function call. If you use a separate set of images, don't forget to create a new XML file for that and update the value in the settings file.

= No Flash support text =

To support visitors without Adobe Flash, you can provide alternative textual content. From the post editor, add the text between `[cover-flow-fx]` and `[/cover-flow-fx]`. From the PHP files of your theme, add the text as *the second argument* of the `coverflowfx_echo_embed_code()` function call.

= If you have PHP4 =

To make it work if you're using PHP4, add the following code `[cover-flow-fx width="600" height="300"][/cover-flow-fx]` in the post editor. From the PHP files of your theme, add the width and height as *the third and fourth argument* of the `coverflowfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/cover-flow.html "Cover Flow FX") is the utility that helps easily customize your Cover Flow FX to fit all your needs.