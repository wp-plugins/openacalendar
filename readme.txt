=== OpenACalendar ===
Contributors: jarofgreen
Tags: events
Requires at least: 3.0.0
Tested up to: 4.0.0
Stable tag: 2.0.8
License: BSD

Incorporate data from an OpenACalendar site into your Wordpress. http://ican.openacalendar.org/

== Description ==

Incorporate data from an OpenACalendar site  (eg http://opentechcalendar.co.uk) into your Wordpress. http://ican.openacalendar.org/

Use a Widget and/or Shortcode to list events.

Ask for help  at: http://ican.openacalendar.org/support.html

== Installation ==

Upload the OpenACalendar plugin to your blog, Activate it.

Note this plugin uses a cron job to regularly get the latest event data. Please make sure cron is running correctly on your WordPress install.

= Setting up =

You need to add an event pool and define some sources.

An event pool is a set of events. You can have several pools and use them seperately, so different pages can show different events.

A source for an event pool tells the plugin where to get it's event data from. One pool can have several sources and all the events will be mixed together.

Upload the OpenACalendar plugin to your blog, Activate it.

Go to Settings, OpenACalendar. Create a new pool with a name.

Add a new source to this pool with the Source URL of a OpenACalendar site (eg "opentechcalendar.co.uk") and any filters you like.

Click "Get events from this source now".

= Widget =

You can then use a widget in the sidebar. The Pool ID you need is displayed on the the settings screen.

= Shortcode =

You can also use a shortcode "openacalendar_events"

Pass attributes:

  * poolid - required. Displayed on the settings screen.
  * descriptionmaxlength - optional, int.
  * usesummarydisplay - optional, boolean. "true" or "false"
  * startformat - optional. String in same format as http://php.net/manual/en/function.date.php
  * eventcount - optional, int.
  * url - optional, string. What URL to use? "site" links to calendar site, "url" links to URL of event.
  * image - optional, string or int. Whether to show an image from the event. One of "normal", "full" or an integer. The integer sets the maximum size of the image in pixels. "full" shows the image as large as possible. "normal" shows the image at the size set by the server.

By default the short code only shows start times, but it can also show end times to:

  * endformat - optional, String in same format as http://php.net/manual/en/function.date.php How to format end time. Defaults to empty.
  * endformatsameday - optional, String in same format as http://php.net/manual/en/function.date.php How to format end time if the event starts and ends on the same day.  Defaults to whatever the value of endformat is.
  * startandenddivider - optional, String. This seperates the start and end times. It defaults to " to ".

Examples:

  * [openacalendar_events poolid=1]
  * [openacalendar_events poolid=2 eventcount=5 startformat="jS F Y"]
  * [openacalendar_events poolid=2 usesummarydisplay="false"]

= Development =

Development happens at: https://github.com/OpenACalendar/OpenACalendar-Web-WordPress


== Changelog ==

= 1.0.0 =
First Version

= 2.0.0 =
  * Events cached in WordPress
  * Shorttag
  * New Widget using cache

= 2.0.1 =
  * Better admin UI
  * Minor improvemments

= 2.0.2 =
  * Can delete source
  * Actually order events!

= 2.0.3 =
  * Can show events a user is attending (Only works on OpenACalendar sites v1.1.5 and up. http://opentechcalendar.co.uk/ and http://hasacalendar.co.uk/ have been upgraded.)

= 2.0.4 =
  * Can pick URL to use
  * Parse usesummarydisplay option to short code properly

= 2.0.5 =
  * Can show end times when using short code

= 2.0.6 = 
  * Bug fix; version 2.0.5 was showing start times instead of end times

= 2.0.7 =
  * Can show image with shortcode

= 2.0.8 =
  * Fix bug when adding source with country https://github.com/OpenACalendar/OpenACalendar-Web-WordPress/issues/47
  * Check country code when adding country https://github.com/OpenACalendar/OpenACalendar-Web-WordPress/issues/45
  * Show better errors when importing data https://github.com/OpenACalendar/OpenACalendar-Web-WordPress/issues/44
  * Mark suitable for WordPress 4


