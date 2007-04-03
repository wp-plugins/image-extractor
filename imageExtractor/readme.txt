=== IMAGE EXTRACTOR ===

Tags: image, resize, 
Contributors: Michele gobbi
Author Website: http://www.dynamick.it
Plugin web page: http://www.dynamick.it/image-extractor-765.html 
Requires at least: 1.5
Tested up to: 1.5
Stable tag: trunk

Image Extractor is a WordPress plugin that extract the first image from the post and display it. 

== Description ==

Image Extractor is a WordPress plugin that extract the first image from the post and display it. 
The plugin main feature is the capability to resize the image found to a destination size. 
The final image is cached in a folder, so you can obtain better performances.

Image Extractor will enable a new template function. It output a complete IMG tag to be inserted into your HTML code. 
The image source is retrieved from the first image found in the current post. 

== Installation ==

1) Download the .zip file and extract it 
2) Upload the extrated folder (imageExtractor/) to the WordPress plugins folder (wp-content/plugins/) 
3) Configure the imageExtractor.php file and set the right cache folder. Make sure it’s writable. 
4) Activate the plugin from the WordPress back office panel

== Syntax ==

The syntax is:

  image_extractor($resize=false, $resize_type=1, $width='', $height='', $class='', $id='', $prefix='', $suffix='')

where:

1) resize: indicate if the plugin has to resize the image and store it in the cache folder 
2) resize_type: there are 3 type of resizing: 

   a) 0 -> image will be resized to the new output size, regardless of the original aspectratio. (default) 
   b) 1 -> image will be cropped if necessary to preserve the aspectratio and avoid image distortions. 
   c)2 -> image will be resized preserving its original aspectratio. differences to the new outputsize will be filled with white 

3) width: the destination width. If resize is false, this property only add/change the WIDTH attribute of the IMG tag 
4) height: the destination height. If resize is false, this property only add/change the HEIGHT attribute of the IMG tag 
5) class: add or change the CLASS attribute of the IMG tag 
6) id: add or change the ID attribute of the IMG tag 
7) prefix: add a prefix to the resulting IMG tag 
8) suffix: append a suffix to the resulting IMG tag 
 

