=== OpenACalendar ===
Contributors: jarofgreen
Tags: events
Requires at least: 3.0.0
Tested up to: 3.9.0
Stable tag: 2.0.1
License: BSD

Incorporate data from an OpenACalendar site into your Wordpress. http://ican.openacalendar.org/

== Description ==

Incorporate data from an OpenACalendar site  (eg http://opentechcalendar.co.uk) into your Wordpress. http://ican.openacalendar.org/

Use a Widget and/or Shortcode to list events.

== Installation ==

Upload the OpenACalendar plugin to your blog, Activate it.

Go to Settings, OpenACalendar. Create a new pool with a name.

Add a new source to this pool with the Source URL of a OpenACalendar site (eg "opentechcalendar.co.uk") and any filters you like.

Click "Get events from this source now".

You can then use a widget in the sidebar. The Pool ID you need is displayed on the the settings screen.

You can also use a shortcode "openacalendar_events"

Pass attributes:

  * poolid - required. Displayed on the settings screen.
  * descriptionmaxlength - optional.
  * usesummarydisplay - optional.
  * startformat - optional.
  * eventcount - optional.

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
