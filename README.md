# New Tab Default Page

![](https://img.shields.io/github/downloads/chrisgrieser/new-tab-default-page/total?label=Total%20Downloads&style=plastic) ![](https://img.shields.io/github/v/release/chrisgrieser/new-tab-default-page?label=Latest%20Release&style=plastic) [![](https://img.shields.io/badge/changelog-click%20here-FFE800?style=plastic)](Changelog.md)

[Obsidian](https://obsidian.md/) plugin to open a note of your choice or the Quick Switcher when creating a new tab, like in the browser.

> **Note**  
> This plugin requires Obsidian 0.16, which is currently only accessible for Obsidian Insiders ([Catalyst License](https://help.obsidian.md/Licenses+%26+Payment/Catalyst+license)).

<!--toc:start-->
  - [Examples for Default New Tab Pages](#examples-for-default-new-tab-pages)
  - [Usage](#usage)
  - [Advanced Examples](#advanced-examples)
    - [Random Quote](#random-quote)
  - [Installation](#installation)
  - [Donate](#donate)
  - [Thanks](#thanks)
<!--toc:end-->

## Examples for Default New Tab Pages
- your homepage note
- your daily note
- a scratchpad note
- trigger a quick switcher
- an image
- a random quote
- …

## Usage
1. Set the note to open in new tabs in the plugin settings. 
2. Set the mode in which the note should open.
3. Open a new tab. 

> **Note**  
> Closing your last tab also opens your new tab page.

## Advanced Examples
### Random Quote
To have a random quote on every new tab, you can use dataview and paste the following code as a dataviewjs-codeblock in a note. 

```js
const quote = JSON.parse(await request("https://api.quotable.io/random"));
dv.span(`> "${quote.content}"  \n> <div style="text-align:end; color:var(--text-muted); font-weight: 600; font-size:90%;">– ${quote.author}</div>`);
```

Then, enter the path of the note in the *New Tab Default Page* settings, and select *Reading Mode*. Now every new note will display a random quote.

### Submit your own idea
Have a cool idea of your own? Feel free to make a PR to this README and submit your own idea.

## Installation
Available in Obsidian's Community Plugin Browser via: `Settings` → `Community Plugins` → `Browse` → Search for *"New Tab Default Page"*

## Donate
<a href='https://ko-fi.com/Y8Y86SQ91' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://cdn.ko-fi.com/cdn/kofi1.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>

## Thanks
Thanks to [@pjeby](https://github.com/pjeby) and various people from the `#plugin-dev` channel for helping me out.
