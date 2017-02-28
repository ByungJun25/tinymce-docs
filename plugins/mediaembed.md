---
layout: default
title: Enhanced Media Embed Plugin
title_nav: Enhanced Media Embed
description: Add rich media previews inside TinyMCE.
keywords: video youtube vimeo mp3 mp4 mov movie clip film spotify
---

The **Enhanced Media Embed** plugin is a [premium TinyMCE plugin](https://tinymce.com/pricing) that will take a URL, send it to a backend service that returns an embeddable snippet of code, and add that code to the editor. That typically takes the form of rich media such as audio, video and social media cards.

## Installation

For the moment the **Enhanced Media Embed** plugin has to be used in conjunction with the [media](../media) plugin, so:

1. Make sure you have the `media` plugin added to the `plugins` list.
2. Add the `mediaembed` plugin to the `plugins` list.

### Example configuration

```js
tinymce.init({
  selector: 'textarea',
  plugins: 'media mediaembed',
  mediaembed_service_url: 'SERVICE_URL',
  mediaembed_max_width: 450
})
```

## Usage

The plugin can be used in two ways, either by simply entering a URL on an empty line and pressing the enter key - or by entering the URL into the media plugin's dialog window. Either way the URL will be handled by the service backend and the returned code will be embedded into the editor.

## Configuration Options

### `mediaembed_service_url`

This setting specifies the URL to the service that will handle your requests and return the embeddable snippets used by the **Media Embed** plugin. You will get the URL as a part of your [premium TinyMCE plugin](https://www.tinymce.com/pricing/) subscription.

### `mediaembed_max_width`

This optional setting specifies a maximum width in pixels of the embedded content. Defaults to `650`.

### `mediaembed_api_key`

This optional setting specifies an API key needed to talk to the service defaults to the global `api_key` setting.

## Downloading Enhanced Media Embed plugin

A [premium TinyMCE plugin](https://www.tinymce.com/pricing/) subscription includes the ability to download and install the **Media Embed** plugin as well as gives you the URL needed to access the service backend.