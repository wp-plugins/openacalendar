=== OpenACalendar ===
Contributors: jarofgreen
Tags: events
Requires at least: 3.0.0
Tested up to: 3.9.0
Stable tag: 2.0.0
License: BSD

Incorporate data from an OpenACalendar site into your Wordpress. http://ican.openacalendar.org/

== Description ==

Incorporate data from an OpenACalendar site into your Wordpress. http://ican.openacalendar.org/

Go to Settings, OpenACalendar. Create a new pool with a name.

Add a new source to this pool with the Source URL of a OpenACalendar site (eg "opentechcalendar.co.uk") and any filters you like.

Click "Get events from this source now".

You can then use a widget in the sidebar. Take the Pool ID from the settings screen.

You can also use a shortcode "openacalendar_events"

Pass attributes:

  * poolid - required, as above
  * descriptionmaxlength - optional
  * usesummarydisplay - optional
  * startformat - optional
  * eventcount - optional

Development happens at: https://github.com/OpenACalendar/OpenACalendar-Web-WordPress

== Installation ==

Upload the OpenACalendar plugin to your blog, Activate it.



== Changelog ==

= 1.0.0 =
First Version

= 2.0.0 =
Events cached in WordPress
Shorttag
New Widget using cache


