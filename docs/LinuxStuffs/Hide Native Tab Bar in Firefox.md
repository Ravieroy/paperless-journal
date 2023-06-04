# Hide native tab bar in Firefox 
In order to hide the tab bar in Firefox, one needs an alternative way to navigate the tabs. The [Tree style tab](https://addons.mozilla.org/en-US/firefox/addon/tree-style-tab/) is one such extension which can be installed for this. After installing Firefox, the following steps can be followed to do that, 

1. Go to `about:support` in the Firefox address bar 
2. Look for your profiles directory and open it:
![[firefox_profile_dir.png]]
3. Create a file named `chrome/userChrome.css` in your profile directory: Use the following command in [[Terminal]]
```bash
mkdir chrome && touch chrome/userChrome.css
```
4. Populate the following CSS code:
```bash
#main-window[tabsintitlebar="true"]:not([extradragspace="true"]) #TabsToolbar > .toolbar-items {
  opacity: 0;
  pointer-events: none;
}
#main-window:not([tabsintitlebar="true"]) #TabsToolbar {
    visibility: collapse !important;
}
#sidebar-box[sidebarcommand="treestyletab_piro_sakura_ne_jp-sidebar-action"] #sidebar-header {
  display: none;
}
.tab {
  margin-left: 1px;
  margin-right: 1px;
 }
```

5. Go to `about:config` in the Firefox address bar. Accept and continue when prompted with risk information
![[firefox_config_caution.png]]

6. Search for *toolkit.legacyUserProfileCustomizations.stylesheets* and toggle it to true. 
![[firefox_stylesheet.png]]

7. Close and restart Firefox browser.

----
