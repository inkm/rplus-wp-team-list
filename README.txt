=== WP Team List ===
Contributors: wearerequired, swissspidy, neverything, hubersen
Donate link: http://required.ch/
Tags: authors, widget, users, list, team, shortcode
Requires at least: 3.5.1
Tested up to: 4.1
Stable tag: 1.0.1
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Display your teammates anywhere on your WordPress site using this easy-to-use plugin.

== Description ==

WP Team List is a plugin that helps you to create a simple team site using your WordPress users with various display options. Either use a shortcode, a template tag or the built-in widget to display blog authors.

After creating similar functionality for a couple of clients, we decided to roll our knowledge into this simple plugin. It's really straightforward to use:

First of all, the plugin adds a small checkbox to the user profile in WordPress to toggle its visibility in the team list. This means you can decide for every user whether he should show up in the team list or not.

You can then use one of these ways to display the list anywhere on your site.

**Template Tag**

Use the `rplus_wp_team_list($args = array(), $echo = true)` function to directly display the users in your teme. If you use `echo = false`, the output is only returned, not echoed.

For example, you can show users of any role ordered by their name:

`<?php rplus_wp_team_list( array( 'role' => 'all', 'orderby' => 'name' ) ); ?>`

Note: WP Team List supports many of the arguments [`WP_User_Query`](http://codex.wordpress.org/Class_Reference/WP_User_Query "WordPress Codex Codex WP_User_Query") supports.

**Shortcode**

The `[rplus_team_list]` shortcode accepts the same arguments as the template tag. Example:

`[rplus_team_list role="Administrator" orderby="post_count" order="desc"]`

This returns all admins ordered by the number of posts they've written (descending).

Pro tip: If you use the [Shortcake WordPress plugin](https://github.com/fusioneng/Shortcake "GitHub - Shortcake"), you'll get an inline preview of the shortcode right in the visual editor. You can also add the shortcode with the click of a button.

**Widget**

Want do display the team members in your sidebar? Use the built-in WordPress widget. You can set the role you want, the number of users to show and even link to a separate team page.

== Installation ==

1. Upload `wp-team-list` to the `/wp-content/plugins/` directory
1. Activate the plugin through the 'Plugins' menu in WordPress
1. Use one of the supported methods (template tag, shortcode, or widget)
1. Optional: Set the visibility status of your users

== Frequently Asked Questions ==

= How do I contribute to WP Team List? =

Easy! You can report bugs, with reproduction steps, or post patches on [GitHub](https://github.com/wearerequired/rplus-wp-team-list).

== Screenshots ==

1. This is how your team list can look like with some additional CSS.
2. The plugin only provides limited styling. It's up for you to adjust it.
3. The configuration options of the built-in widget.

== Changelog ==

= 1.0.1 =
* Fix: Updated textdomain to match the plugin slug

= 1.0.0 =
* Initial Release

== Upgrade Notice ==

= 1.0.1 =
We changed the plugin's textdomain to improve translation handling.

= 1.0.0 =
Initial Release