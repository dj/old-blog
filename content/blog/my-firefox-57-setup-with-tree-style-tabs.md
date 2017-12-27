---
date: 2017-12-27T18:59:00.183Z
title: My Firefox 57 Setup With Tree Style Tabs
---
![Screenshot of Firefox 57 with Tree Style Tabs extension](/images/uploads/Screen Shot 2017-12-27 at 1.21.07 PM.png)

## Add-ons are dead, long live WebExtensions

Firefox 57 deprecates the old Firefox add-on ecosystem in favor of the new standard WebExtensions. I've never really liked using too many browser extensions, personally. On top of possible security or performance issues they can introduce, I also worried about getting locked in to one browser because of growing attached to one extension.

Well, my fears have come true. After using Tree Style Tabs I'm not sure I could ever go back to using a normal, horizontal tab bar again!

## Tweaking the UI with userChrome.css

![Screenshot of Firefox 57 with default UI and Tree Style Tabs](/images/uploads/Screen Shot 2017-12-27 at 2.09.45 PM.png)

This is what Tree Style Tabs looks like without any customization. Ideally, we should be able to hide the horizontal Tabs Toolbar on top either in Firefox's options or the Tree Style Tabs options. Mozilla has said that they want to [provide a robust Tab API](https://blog.mozilla.org/addons/2017/11/03/keeping-tabs-tab-api/). I'll probably come back and update this blog post when this is possible without `userChrome.css` but maybe check [this ticket](https://blog.mozilla.org/addons/2017/11/03/keeping-tabs-tab-api/) to see if it's been resolved.

In the meantime, we can add a file to our Firefox profile to customize Firefox with css.

1. Download [Firefox 57](https://www.mozilla.org/en-US/firefox/new/)
2. Install [Tree Style Tabs](https://addons.mozilla.org/en-US/firefox/addon/tree-style-tab/)
3. Navigate to `about:support` in Firefox.
4. Click the button to the right of "Profile Folder"
5. Inside of your profile folder, add a folder called `chrome` and inside that create a file called `userChrome.css` and add the following contents

<script src="https://gist.github.com/dj/2ab3aa20fa1076d4e28dfcc6d1e519c3.js"></script>

Viola! Restart Firefox and you should have a beautiful, Tab Toolbar-free UI.
