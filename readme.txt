=== Simple SSL ===
Tags: SSL, https, force SSL, mixed content, insecure content, secure website, website security, TLS, security, secure socket layers, HSTS, simple ssl
Requires at least: 4.6
Tested up to: 5.4
Requires PHP: 5.4
License: GPL2

No setup required! You only need an SSL certificate, and this plugin will do the rest.

== Description ==
Simple SSL automatically detects your settings and configures your website to run over https.
To keep it lightweight, the options are kept to a minimum. The entire site will move to SSL.

== Installation ==
To install this plugin:

1. Make a backup!
2. Install your SSL certificate
3. Download the plugin
4. Upload the plugin to the wp-content/plugins directory,
5. Go to “plugins” in your WordPress admin, then click activate.
6. You will now see a notice asking you to enable SSL. Click it and log in again.

== Frequently Asked Questions ==

= What are simple simple steps for setup? =
* Get an SSL certificate (can't do that for you, sorry.)
* Activate this plugin
* Enable SSL with one click

Always backup before you go! 

= What does the plugin actually do? =
* The plugin handles most issues that WordPress has with SSL, like when you're behind a reverse proxy/loadbalancer, or when no headers are passed which WordPress can use to detect SSL.
* All incoming requests are redirected to https. Default with an internal WordPress redirect, but you can also enable a .htaccess redirect.
* The siteurl and homeurl are changed to https.
* Your insecure content is fixed by replacing all http:// URL's with https://, except hyperlinks to other domains. Dynamically, so no database changes are made (except for the siteurl and homeurl).

= Does the mixed content fixer make my site slower? =
On a site where the source consists of about 60.000 characters, the delay caused by the mixed content fixer is about 0.00188 seconds. If this is too much for you, fix the mixed content manually and deactivate it in the settings.

= Is the plugin multisite compatible? =
Yes. There is a dedicated network settings page where you can switch between network activated SSL and per page SSL. In the dedicated pro for multisite plugin, you can override all site settings for SSL on the network level, and can activate and deactivate SSL in the network menu for each site.

== Changelog ==
= 1.0.0 =
* Initial release

= 2.0.0 =
* Additional functionalities added