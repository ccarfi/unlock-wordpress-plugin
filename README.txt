=== Unlock Protocol ===
Contributors: julien51
Donate link: https://donate.unlock-protocol.com/?r=unlock-protocol/unlock
Tags: paywall, ethereum, monetization, unlock, membership, subscription, member
Requires at least: 5.1
Tested up to: 5.3
Requires PHP: 7.2
Stable tag: 2.0
License: GPLv3
License URI: https://github.com/unlock-protocol/unlock-wordpress-plugin/blob/master/LICENSE

This plugin lets authors adds locks to theit posts and pages so that only paying visitors can view their content.

== Description ==

[Unlock](https://unlock-protocol.com/) is a protocol for memberships which lets any creator monetize their content in a permissionless way.

You can [try a demo on this site](https://wordpress-demo.unlock-protocol.com/) where the content of the post changes on whether the visitor is a member or not.

In order to become members, visitors need to be using a web3 enabled wallet such as [MetaMask](https://metamask.io/) or a web browser with an embeded wallet, such as [Opera](https://www.opera.com/crypto). They also need a balance of Ether in order to purchase keys to pay for the memberships. Ether can be bought on exchanges such as [Coinbase](https://www.coinbase.com/).

== Getting Started ==

If you'd like to add a lock to your site, start by [deploying your first lock](https://unlock-protocol.com/blog/create-first-lock/).

While the lock is deploying you should [download this plugin](https://wordpress.org/plugins/unlock-protocol/) from the Wordpress site. Then, from the administration of your Wordpress.org website, in the `Plugins` section, click on the `Add New` button and then on the `Upload Plugin` button to upload the plugin.

== Writing locked stories ==

First you will need to add the lock configuration for each post or page to which you will add locked content.
This can be done in the `Document` tab of the Editor. There look for the `Unlock Protocol Configuration` pane and add the required configuration. Check Unlock's docs for available options.

Here is an example:
```
{ locks: { '0xB0114bbDCe17e0AF91b2Be32916a1e236cf6034F': { } }, callToAction: { } }
```

The plugin provides you with "Blocks" which can be used in the Gutenberg Editor, for both posts and pages. We provide 2 different blocks:

- The "Unlock" block: a block whose content (and nested blocks) can be set to be visible to only members or non-members. Each block can be customized

- The "checkout button" block: a block with a button to let you add a button for people to become members. It is recommended to put this button inside of a block only visible to non-members!

Once your story includes the content you need, you can preview its content like any other WordPress post or page. We recommend the use of a web3 wallet which supports multiple accounts so that you can easily toggle between accounts which are already members and accounts which are not members yet!

== Contributing ==

This plugin is, like all of the Unlock code, [open source](https://github.com/unlock-protocol/unlock-wordpress-plugin). You're encouraged to fork it and make any changes you'd like! If you believe these changes would be beneficial to others, we encourage you to also open a Pull Request so that we could add these to the main branch released on the wordpress.org website!

In order to update the plugin, check out the current subversion state with

    svn co  https://plugins.svn.wordpress.org/unlock-protocol

Then checkout the git repo inside of `trunk` and commit the changes into svn with:

    svn ci -m "commit message"

Then, tag the new version (replace X and Y!) to release it:

    svn cp trunk tags/X.Y
    svn ci -m "tagging version X.Y"

== Frequently Asked Questions ==

To be completed with questions!

== Changelog ==

= 2.1 =
* Uses the latest Unlock paywall script https://unlock-protocol.com/blog/introducing-latest-paywall/

= 2.0 =
* each post/page can have a different configuration
* block setting is now visible inside of the Editor

= 1.6 =
Button is not only visible when content is locked

= 1.5 =
Cleanup

= 1.1 =
Supporting nested blocks.

= 1.0 =
Initial version

== Upgrade Notice ==

N/A

