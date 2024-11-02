=== Block Common Crawl via robots.txt ===
Contributors: apasionados
Donate link: https://apasionados.es/
Author URI: https://apasionados.es/
Tags: robots, robots.txt, crawler, robot, bot, seo
Requires at least: 5.9
Tested up to: 6.3
Requires PHP: 7.4
Stable tag: 1.0.0
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Blocks the Common Crawl bot (CCBot) that gathers data that is used to train AI algorithms like ChatGPT through the WordPress virtual robots.txt file

== Description ==

This plugin adds lines to the virtual robots.txt file that WordPress creates automagically if the file is not present physically on the server to block the Common Crawl bot (CCBot) that is used to train AI algorithms like ChatGPT (in version 3.5 it makes up 60% of the training data mix) to crawl websites. Here is the [information about the Common Crawl bot (CCBot)](https://commoncrawl.org/big-picture/frequently-asked-questions/).

> Please be aware of what this plugin does exactly: If you activate the plugin it will add some lines to the robots.txt file to tell Common Crawl bots to **not to crawl and index** parts of this website.

**Please only activate this plugin if you know what you're doing**.

= What can I do with this plugin? =

This plugin adds the necessary lines to the virtual robots.txt file that WordPress creates automagically to block the Common Crawl bot (CCBot) is used to train AI algorithms like ChatGPT to crawl websites.

= What ideas is this plugin based on? =

Our plugin to [block the OpenAI ChatGTP bot](https://wordpress.org/plugins/block-chat-gpt-via-robots-txt/) after the launch of the OpenAI ChatGPT plugins that crawl websites.

= What is the robots.txt file? =

The robots.txt file is a plain text file located at the root folder of a domain (or subdomain) which tells web crawlers (like Googlebot) what parts of the website they should access and index.

The first thing a search engine crawler looks at when it is visiting a page is the robots.txt file and it controls how search engine spiders see and interact with the web pages.

= System requirements =

PHP version 7.4 or greater.
We require 7.4 or higher because we believe that everybody should be running a modern PHP version. When releasing this plugin [Wordpress recommends PHP 7.4 or higher](https://wordpress.org/about/requirements/). We would recommend 8.0 or higher as 7.4 has no security updates since 28 Nov 2022.

= How to get this plugin in your Language! =
The first release is avaliable in English and Spanish. In the "languages" folder we have included the necessary files to translate this plugin.

If you would like the plugin in your language and you're good at translating, please use the [native WordPress Translation](https://translate.wordpress.org/) functionality.

New to Translating a plugin? First read through the [Translator Handbook](https://make.wordpress.org/polyglots/handbook/tools/glotpress-translate-wordpress-org/), then select your locale at [Translating WordPress](https://translate.wordpress.org/) and finally go to the [translation page for this plugin](https://translate.wordpress.org/projects/wp-plugins/block-ecommerce-assets-via-robots-txt/) to translate it.

= Further Reading =
You can access the description of the plugin in Spanish at: [Block Common Crawl bot (CCBot) via robots.txt en espa&ntilde;ol](https://apasionados.es/blog/).

== Screenshots ==

1. Lines that the plugin adds to the virtual robots.txt file that WordPress creates.

== Installation ==

1. First you will have to upload the plugin to the `/wp-content/plugins/` folder.
2. Then activate the plugin in the plugin panel. There are no settings.

== Frequently Asked Questions ==

= Why did you make this plugin?  =
We created this plugin to be able to append the lines to block the access of the Common Crawl bot (CCBot) to the website via robots.txt without having to upload a robots.txt file.

= Does Block Common Crawl bog via robots.txt make changes to the database? =
No. The plugin doesn't write any options or settings to the database.

= How can I check out if the plugin works for me? =
Install and activate. Have a look at the content of the robots.txt file in root of the domain.

= How can I remove Block Common Crawl bog via robots.txt? =
You can simply activate, deactivate or delete it in your plugin management section. There are no options stored in the database so you can delete it also via FTP and everything will be removed.

= What happens if there is a physical robots.txt file on the server? =
**This plugin makes changes to the virtual robots.txt file generated automagically by WordPress and doesn't work with a physical robots.txt file**. In order to use this plugin you need to remove the physical robots.txt file from your server. Please delete the robots.txt file via FTP or Server Panel before using this plugin. **We check this on activation (and only on activation)**. If we find a physical robots.txt file the plugin can't be activated until the file is removed. Please keep in mind that we only check it on plugin activation and after activation we don't check it any more; so if you upload a robots.txt file to the root of the domain once the plugin is activated, the plugin will have no effects but you will not receive a warning.

= What happens if WordPress is installed in a subdirectory? =
**WordPress must be installed in top-level directory of the web server.** Please note that the robots.txt must be in the top-level directory of your web server. If WordPress is installed in a subdirectory this plugin will not be effective because the robots.txt file generated by WordPress in the subdirectory will be ignored by the bots. Please note that we don\'t check this. You can read more about the robots.txt standard here [robotstxt.org: How to create a /robots.txt file and Where to put it](http://www.robotstxt.org/robotstxt.html).

= Are there any known incompatibilities? =
Please don't use it with *WordPress MultiSite*, as it has not been tested.

The plugin has similar functionality as the [Virtual Robots.txt](https://wordpress.org/plugins/pc-robotstxt/) and the [Better Robots.txt – Index, Rank & SEO booster](https://wordpress.org/plugins/better-robots-txt/) plugin; **both are not compatible with our plugin** as they remove all the virtual WordPress robots.txt content and create their own. The directives our plugin creates are not added to the robots.txt file these plugins generate as they don't use the standard functions of WordPress to append information to them.

The plugin can be used along our plugin to [block the OpenAI ChatGTP bot](https://wordpress.org/plugins/block-chat-gpt-via-robots-txt/).

= What lines does this plugin add to the robots.txt file? =
User-agent: CCBot
Disallow: /

= Are there any server requirements? =
Yes. The plugin requires a PHP version 7.4 or higher and we recommend using PHP version 7.4 or higher. The plugin has been tested with PHP up to 7.4. When releasing this plugin [Wordpress recommends PHP 7.4 or higher](https://wordpress.org/about/requirements/).

= Do you make use of Block Common Crawl (CCBot) via robots.txt yourself? = 
Of course we do. That's why we created it. ;-)

== Changelog ==

= 1.0.0 (21/APR/2023) =
* First release.

== Upgrade Notice ==

= 1.0.0 =
FIRST RELEASE

== Contact ==

For further information please send us an [email](https://apasionados.es/contacto/index.php?desde=wordpress-org-block-chatgpt-assets-via-robots-txt).