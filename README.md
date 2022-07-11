# Workchat Profanity Filter Plugin (Beta)

This plugin allows you to censor profanity on your Workchat server. The plugin checks all messages for matches against the configured "Bad words list" before they are posted to any channel. The characters in any word matches are replaced with a series of "\*"s.

**Supported Workchat Server Versions: 5.2+**

## Plugin Marketplace

1. Go to **Main Menu > Plugin Marketplace** in Workchat.
2. Search for "Profanity Filter" or manually find the plugin from the list and click **Install**
3. Once the plugin has downloaded and been installed, click **Configure**.

## Manual Installation

1. Go to the [releases page of this Github repository](https://gitlab.com/w1572/workchat-plugin-profanity-filter/releases) and download the latest release for your Workchat server.
2. Upload this file in the Workchat System Console under **System Console > Plugins > Management** to install the plugin. To learn more about how to upload a plugin.
3. Activate the plugin at **System Console > Plugins > Management**.

### Usage

You can edit the bad words list in **System Console > Plugins > Profanity Filter > Bad words list**.
In this list, you can use Regular Expressions to match bad words. For example, `bad[[:space:]]?word` will match both `badword` and `bad word`.

Choose to either censor the bad words with a character or reject the post with a custom warning message:

![Post rejected by the plugin](./images/post-rejected.gif)

![Post censored by the plugin](./images/post-censored.gif)
