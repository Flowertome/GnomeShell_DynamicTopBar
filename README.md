# DISCLAIMER

This extension was usefull back in the days, but now that Gnome has included a similar feature I didn't need it anymore. If you want to takeover the maintenance and the development feel free to open an issue to discuss that topic.

I will only continue to merge pull-request for translations, maybe bugfixes or new features, but I will not fix bugs or implement new features myself.

---

Dynamic Top Bar
===============

Dynamic Top Bar is a Gnome Shell extension
that make the top bar transparent when no
window is maximized.

Demo
====
![GIF Demo](https://feildel.fr/gnome-shell/dynamic-status-bar.gif)

How-To Install
==============

Download
--------
You can download this extension with various methods:

- from [Gnome website](https://extensions.gnome.org/extension/885/dynamic-top-bar/)
- Using the latest release posted on GitHub https://github.com/AMDG2/GnomeShell_DynamicTopBar/releases
- By cloning the repo

Install
-------
Just past the `dynamicTopBar@gnomeshell.feildel.fr`
folder to `~/.local/share/gnome-shell/extensions`
then activate the extensions with Gnome Tweak Tool
for example.

```bash
cp -r dynamicTopBar@gnomeshell.feildel.fr ~/.local/share/gnome-shell/extensions
gnome-shell-extension-tool -e dynamicTopBar@gnomeshell.feildel.fr
```
Might require a Gnome restart. Press ALT+F2 and type 'r' and hit enter.

Or you can use the `install.sh` script.

If you want to install this extension to the directory: '/usr', use the following command to pass in the parameters.
```bash
./install.sh root
```
If you want to install this extension to the directory: '$HOME/.local', use the following command.
```bash
./install.sh
```

Theme compatibility
===================

Not all theme are compatible with this extension.

- If you are a theme developer please read the following paragraph.
- If you are a theme user and the extension seems broken please report the issue in this repository and to the theme developer

Theme developer information
----------------------------

If your theme use images to style the panel look it won't be compatible with the extension without work.

The extension only style the `background-color` property of the panel. But your theme may use the following classes to detect when the panel should be transparent or gradient :

- `dynamic-top-bar-transparency`
- `dynamic-top-bar-gradient`
