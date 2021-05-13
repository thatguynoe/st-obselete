# Noe's build of st

My build of st is heavily inspired by [Luke Smith's build](https://github.com/LukeSmithxyz/st), which I strongly encourage you to check out for more info.

## Bindings

* **scroll** with `alt-j`, `alt-k` or `alt-pgup`, `alt-pgdn` or `alt-↑`, `alt-↓`. Scroll faster with `alt-u`, `alt-d`.
* **change font size** with the same bindings as above, but with holding down shift. Reset with `alt-home`.
* **change transparency** with `alt-a`, `alt-s`.
* **copy text** with `alt-y`, **paste** with `alt-p` or `shift-insert`.
* **copy command output** with `alt-o`, **open urls** with `alt-l`, and **copy urls** with `alt-i`.

## Patches and features:

* [**alpha-0.8.2**](https://st.suckless.org/patches/alpha/st-alpha-0.8.2.diff) provides transparency---make sure you have a composite manager (such as `xcompmgr` or `picom`) installed for this to work.
* [**anysize-0.8.1**](https://st.suckless.org/patches/anysize/st-anysize-0.8.1.diff) allows st to fill the entire space allocated to it.
* [**bold-is-not-bright-20190127-3be4cf1**](https://st.suckless.org/patches/bold-is-not-bright/st-bold-is-not-bright-20190127-3be4cf1.diff) is self-explanatory.
* [**boxdraw_v2-0.8.3**](https://st.suckless.org/patches/boxdraw/st-boxdraw_v2-0.8.3.diff) renders lines/blocks characters better.
* [**externalpipe-0.8.4**](https://st.suckless.org/patches/externalpipe/st-externalpipe-0.8.4.diff) provides functionality for opening and copying urls.
* [**font2-20190416-ba72400**](https://st.suckless.org/patches/font2/st-font2-20190416-ba72400.diff) adds support for multiple fonts.
* [**gruvbox-dark-0.8.2**](https://st.suckless.org/patches/gruvbox/st-gruvbox-dark-0.8.2.diff) enables the gruvbox theme.
* [**scrollback-20201205-4ef0cbd**](https://st.suckless.org/patches/scrollback/st-scrollback-20201205-4ef0cbd.diff) allows for scrolling in st.
* [**vertcenter-20180320-6ac8c8a**](https://st.suckless.org/patches/vertcenter/st-vertcenter-20180320-6ac8c8a.diff) vertically centers lines.

## Installation

```
git clone https://github.com/thatguynoe/st
cd st
sudo make install
```

## Please install `libxft-bgra`<sup>`aur`</sup>!

In order for st to display color emojis, the `libxft-bgra`<sup>`aur`</sup> package must be installed---else, st will crash.