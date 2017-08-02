=== YouList - YouTube playlist shortcode  ===
Contributors: birgire
Donate link: https://www.paypal.com/is/cgi-bin/webscr?cmd=_flow&SESSION=oKt0477jvHqLRssQCQmB_Oas5csxlh316mkBM4p9soLqQ3o-wfIuZPzqdQy&dispatch=5885d80a13c0db1f8e263663d3faee8d7283e7f0184a5674430f290db9e9c846
Tags: youtube, shortcode, embed, playlist, youtube playlist
Requires at least: 3.0
Tested up to: 3.4.1
Stable tag: 1.0.5
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

A simple shortcode to embed playlists or handpicked videos in a single YouTube&trade; player. 

== Description ==

This plugin adds the shortcode [youlist] so you can easily embed  YouTube&trade; playlist defined by

* playlist id (PL in front of the playlist id)
* comma seperated video ids list
* user favorites 
* user uploads
* search query

in a single YouTube&trade; player.

[Live demo](http://xlino.com/projects/youlist-youtube-playlist-shortcode-plugin/)

= New in version 1.0.5 =

* enable nocookies
* enable the https protocol
* play videos in a specific quality (fx. hd720)
* enable wmode to handle z-index issues.

= Usage Examples =

To embed a playlist with thumbnails 
`[youlist pid="PL3FF15AA7ED356D9F"]`

To embed three videos with thumbnails (comma seperated video id list):
`[youlist vid="ZF_K8D414-Y,sFHXWoawnt0,E2uOGOqIyC4"]`

To embed three videos without thumbnails:
`[youlist vid="ZF_K8D414-Y,sFHXWoawnt0,E2uOGOqIyC4" showinfo="0"]`

To embed a playlist from the search string "higgs boson"
`[youlist search="higgs boson" width="600" height="400"]`

To embed a playlist for all uploaded videos for the user "mismag822"
`[youlist uid="mismag822" listtype="user_uploads"]`

To embed a playlist for all favorite videos for the user "mismag822"
`[youlist uid="mismag822" listtype="user_favorites"]`

To embed a playlist width your own custom style
`[youlist pid="PL3FF15AA7ED356D9F" style="width:300px;height:400px;z-index:1;"]`

To embed a user playlist with all the supported attributes (default values shown):
`[youlist 
	uid="mismag822" 
	showinfo="1" 
	width="680" 
	height="480" 
	class="youlist"
	autohide="2"
	autoplay="0"
	disablekb="0"
	listtype="user_uploads"
	theme="dark" 
	modestbranding="1" 
	controls="1" 
	color="red" 
	fs="1" 
	rel="1" 
	start="0" 
	loop="0" 
	iv_load_policy="1" 
	version="3"
	style="" 	
	vq="" 	
	nocookie="0"
	https="0" 	
	wmode="" 	
	parameters="" 	
]`


= Ideas for how to use this plugin =

 1. You can use it to display ad-video before or after the main video
 1. You can have your own short trailer before the main video
 1. You can collect lessons/tutorials/music videos
 1. You can use it for your YouTube&trade; playlist
 1. You can watch your friends favourites videos
 1. You can collect videos for your kid and watch it on your site
 1. ... etc ...

= Shortcode Parameters = 

The youList-shortcode is a wrapper for most of the YouTube&trade; iframe parameters described here:

https://developers.google.com/youtube/player_parameters

**iframe parameters:**

* width [integer] - iframe width in pixels
* height [integer] - iframe height in pixels
* class  [string] - iframe css classname
* style [string] - iframe css custom style
* parameters [string] - custom source parameters (&param1=value1&...)

**youtube parameters:**

* pid [string] - YouTube playlist ID
* uid [string] - YouTube user ID)
* vid [string] - Comma seperated YouTube Videos ID list
* listtype [playlist|user_uploads|search] - YouTube listtype
* search  [string] - YouTube search string)
* theme [dark|light] - Dark or light control bar
* modestbranding [0|1] - Prevent the YouTube logo from displaying in the control bar
* showinfo [0|1] - Display thumbnail images for the videos in the playlist
* autohide [0|1|2] - Hide the video controls automatically after a video begins playing
* autoplay [0|1] - The initial video will autoplay when the player loads
* disablekb [0|1] - Disable the player keyboard controls
* controls [0|1|2] - Display the video player controls
* color [red|white] - The color in the video progress bar 
* fs [0|1] - Display the fullscreen button
* rel [0|1] - Show related videos when playback of the initial video ends
* start [integer] - Play the video at the given number of seconds from the start of the video
* loop [0|1] - Play the entire playlist and then start again at the first video
* iv_load_policy [1|3] - Show video annotations
* version [2|3] - AS player version
* https [0|1] - Enable the https protocol
* nocookie [0|1] - No cookies thank you
* vq [small|medium|large|hd720|hd1080] - Change video quality

== Installation ==

= Installation =

 1. Upload the plugin directory to the `/wp-content/plugins/` directory or use the installer via backend of WordPress
 1. Activate the plugin through the 'Plugins' menu in WordPress

== Frequently Asked Questions ==

[Check out the support forum](http://wordpress.org/support/plugin/youlist)

== Screenshots ==

1. YouTube playlist with thumbnails.

More screenshots [here](http://xlino.com/projects/youlist-youtube-playlist-shortcode-plugin/)

== Changelog ==

= 1.0.5 =

* added: vq parameter to change the video quality, (fx hd720) (Props cjgrasso)
* added: https parameter to enable the secure protocol
* added: nocookie parameter to disable cookies
* added: wmode parameter to handle z-index issues (Props patmak)
* added: parameters parameter for custom parameters
* changed: updated the readme.txt with better description of the parameters

= 1.0.2 =

* added: [youlist] shortcodes can now be used in text-widgets
* added: custom iframe style attribute
* fixed: added the missing parameters audohide and audoplay
* changed: new usage example in the readme.txt file

= 1.0.1 =

* added: new attributes: listtype, autohide, autoplay, disablekb
* added: possibility to display user's favorites playlist
* changed: updated he readme.txt file with new usage examples

= 1.0.0 =
 
* Initial Release
 
