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
  * descriptionmaxlength - optional.
  * usesummarydisplay - optional.
  * startformat - optional.
  * eventcount - optional.

Examples:

  * [openacalendar_events poolid=1]
  * [openacalendar_events poolid=2 eventcount=5 startformat="jS F Y"]

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
