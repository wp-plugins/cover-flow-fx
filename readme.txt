=== Cover Flow FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, cover, flow, coverflow, itunes, free, flash, page, slide, portfolio, book, flip, gallery, slideshow, auto, scroll, rotator, scroller, tooltip, text, 3d, scrollbar, image, effect, preloader, as3, horizontal
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

One of the most advanced Cover Flows on the web. Completely XML customizable without any Flash knowledge. And it's free!

== Description ==

The Cover Flow FX can be embedded in any website for free without even using Flash and it can have an overall width and height up to 1680 x 1050 pixels. I uses the Papervision3D engine and has multiple plane and camera views. It supports all types of images (JPG, GIF, BMP, PNG) which can have different sizes - they will be automatically adjusted to fit in the same height. It has an auto play function with external PNGs (customizable) for play/pause buttons. Optional scroll bar with multiple skins to choose from. Extensive configurations for tooltip and reflection.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/cover-flow-fx.zip "Cover Flow FX Plugin") (that you have to install and activate) & [Free archive](http://www.flashxml.net/free/download/cover-flow.zip "Cover Flow FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **cover-flow-fx** and copy the content of the **free archive** there
3. If you copied the **free archive** to a location different than the one above, go to **Cover Flow FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[cover-flow-fx][/cover-flow-fx]` where you want the Flash to show up in your post/page
5. If you want to make the Cover Flow FX part of your theme, edit the template files and add `<?php coverflowfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Cover Flow FX](http://www.flashxml.net/cover-flow.html "Cover Flow FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/cover-flow-fx/settings.xml`
7. To use your own images, upload them to `wp-content/flashxml/cover-flow-fx/images/` and update the `wp-content/flashxml/cover-flow-fx/images.xml` file accordingly

= Additional settings file =

To embed the Cover Flow FX more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called `settings2.xml`. Add `[cover-flow-fx settings="settings2.xml"][/cover-flow-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `coverflowfx_echo_embed_code()` function call (for example `<?php coverflowfx_echo_embed_code("settings2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[cover-flow-fx]` and `[/cover-flow-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `coverflowfx_echo_embed_code()` function call (for example `<?php coverflowfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[cover-flow-fx width="600" height="300"][/cover-flow-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `coverflowfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/cover-flow.html "Cover Flow FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/cover-flow-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/cover-flow.html "Cover Flow FX") is the utility that helps easily customize your Cover Flow FX to fit all your needs.