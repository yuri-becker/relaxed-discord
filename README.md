<a name="readme-top"></a>
[![GPL License](https://img.shields.io/github/license/yuri-becker/relaxed-discord?style=for-the-badge)](https://github.com/yuri-becker/relaxed-discord/blob/main/LICENSE)

<br />
<div align="center">

<h1 align="center"><strong>Relaxed Discord</strong></h1>

<p align="center"> 
    Discord theme providing some adjustments to make it less cluttered.<br/>
    Use with Discord mods like <a href="https://github.com/BetterDiscord/BetterDiscord">BetterDiscord</a> or <a href="https://github.com/Vendicated/Vencord">Vencord</a>.
</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#installation">Installation</a>
      <ul>
        <li><a href="#vencord">Vencord</a></li>
        <li><a href="#betterdiscord">BetterDiscord</a></li>
        <li><a href="#usage-with-other-themes"> Usage with other themes</a></li>
      </ul>
    </li>
    <li><a href="#chat-background">Chat Background</a></li>
    <li><a href="#list-of-adjustments">List of Adjustments</a></li>
    <li><a href="#contributions">Contributions</a></li>
  </ol>
</details>
<br/>

## Installation

### Vencord

Go to `Settings` → `Vencord > Themes` → `Online Themes` and paste this URL at the end:

```
https://yuri-becker.github.io/relaxed-discord/RelaxedDiscord.theme.css
```

### BetterDiscord

1. Download <a href="https://yuri-becker.github.io/relaxed-discord/RelaxedDiscord.theme.css" download>the theme</a> (Right Click → Save Link as...).
2. Go to `Settings` → `BetterDiscord > Themes` and open your theme folder using the folder icon on the top left.
3. Move `RelaxedDiscord.theme.css` to the theme folder.
4. After Relaxed Discord pops up, enable it using the toggle switch on the right.


### Usage with other themes

This theme is generally **compatible with other themes**, since all it contains are a few tweaks.

To make sure that the tweaks in this theme are not overridden by your "main" theme, **put this theme at the end** of your themes list.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Chat background

This theme supports setting a background for chats. If you don't want a background, just skip this.

First upload the image somewhere (I recommended just posting it in a private Discord chat) or copy the URL if the image is already online. 

Then you need to open your QuickCSS/<whatever it is called on BD>.

On **Vencord**, go to `Settings` → `Vencord > Themes` → `Load Themes` → `Edit QuickCSS`

On **BetterDiscord**, go to `Settings` → `BetterDiscord > Custom CSS` (make sure to click the save icon after you've finished your edits).

Having this opened, set the image url like this:

```css
:root {
  --relaxed-background-image: url("https://images.unsplash.com/photo-1554668048-5055c5654bbc?ixlib=rb-4.0.3&q=85&fm=jpg&crop=entropy&cs=srgb&dl=pawel-czerwinski-xWSUI7tpiTY-unsplash.jpg");
}
```

If you want to change the filters applied to the background, set them like this:

```css
:root {
  --relaxed-background-image: url("https://images.unsplash.com/photo-1554668048-5055c5654bbc?ixlib=rb-4.0.3&q=85&fm=jpg&crop=entropy&cs=srgb&dl=pawel-czerwinski-xWSUI7tpiTY-unsplash.jpg");
  /* Add this line next to your --relaxed-backgroud-image definition */
  --relaxed-background-image-filter: brightness(25%) blur(10px);   
}
```

 See [the docs for filter](https://developer.mozilla.org/en-US/docs/Web/CSS/filter) about possible values.

<p align="right">(<a href="#readme-top">back to top</a>)</p>


## List of Adjustments

* Add background to chats.<br/>
  Simply for aesthetics.

* Restrict chat message width to about 80 characters.<br/> 
  By default, when you get/write walls of text, Discord just spans the text over the entire available width. Which is pretty long even on my 14 inch notebook. Lines that are too wide make it hard to focus on the text. By restricting the line width, reading the text will be less straining for most people. (Its a pet peeve of mine, that's why I'm being so verbose about it.)

* Remove gift button in message field.<br/>
  Now you can't buy your friends Nitro anymore!

* Add margin in Direct Messages list.<br/>
  Just to make it less dense, I personally don't need to keep track of that many conversations at once.

* Add margin in Friends list.<br/>
  Same reason - I found it a bit too dense.

* Add margin and remove tile background of Active Now column.<br/>
  Just found it more neat this way.

* Correct cursor when hovering over your name on the bottom left.<br/>
  For some reason, only the avatar has a pointer cursor although the entire area is clickable

* Remove status text under own name on the bottom left.<br/>
  I don't need to see my own status to be honest.

* Remove Help icon in the top bar.<br/>
  Cool people don't need help. 😎

* Align profile container and chat container<br/>
  The thing from the March 2025 UI update.

<p align="right">(<a href="#readme-top">back to top</a>)</p>


## Contributions

If you want to suggest a change, you're welcome to [Open an Issue](https://github.com/yuri-becker/relaxed-discord/issues/new).

As of now, this theme isn't doing much but I'm willing to let it grow, fix more usability issues and decrease the mental load experienced when using Discord.

<p align="right">(<a href="#readme-top">back to top</a>)</p>
