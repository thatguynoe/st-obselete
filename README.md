# Noe's build of st

My build of st is heavily inspired by [Luke Smith's build](https://github.com/LukeSmithxyz/st), which I strongly encourage you to check out for more info. Running on commit [`2c5edf28ec851907305d73c6218ce75d39f1767f`](https://git.suckless.org/st/commit/2c5edf28ec851907305d73c6218ce75d39f1767f.html).

## Bindings

* **scroll** with <kbd>alt-j</kbd>, <kbd>alt-k</kbd> or <kbd>alt-pgup</kbd>, <kbd>alt-pgdn</kbd> or <kbd>alt-↑</kbd>, <kbd>alt-↓</kbd>. Scroll faster with <kbd>alt-u</kbd>, <kbd>alt-d</kbd>.
* **change font size** with the same bindings as above, but with holding down shift. Reset with <kbd>alt-home</kbd>.
* **change transparency** with <kbd>alt-a</kbd>, <kbd>alt-s</kbd>.
* **copy text** with <kbd>alt-y</kbd>, **paste** with <kbd>alt-p</kbd> or <kbd>shift-insert</kbd>.
* **copy command output** with <kbd>alt-o</kbd>, **open urls** with <kbd>alt-l</kbd>, and **copy urls** with <kbd>alt-i</kbd>.

## Patches and features

* [**alpha-0.8.2**](https://st.suckless.org/patches/alpha/st-alpha-0.8.2.diff) provides transparency---make sure you have a composite manager (such as `xcompmgr` or `picom`) installed for this to work.
* [**bold-is-not-bright-20190127-3be4cf1**](https://st.suckless.org/patches/bold-is-not-bright/st-bold-is-not-bright-20190127-3be4cf1.diff) is self-explanatory.
* [**boxdraw_v2-0.8.3**](https://st.suckless.org/patches/boxdraw/st-boxdraw_v2-0.8.3.diff) renders lines/blocks characters better.
* [**changealpha-0.8.5**](https://github.com/LukeSmithxyz/st/commit/73a6020865607018f6442317e7f94fb5d54a7016) lets you change transparency on the fly.
* [**columnredraw-0.8.4**](https://github.com/nimaipatel/st/blob/master/patches/7672445bab01cb4e861651dc540566ac22e25812.diff) prevents cutting off text after resizing.
* [**csi_22_23-0.8.4**](https://st.suckless.org/patches/csi_22_23/st-csi_22_23-0.8.4.diff) saves and restores the window title (e.g. when opening and closing neovim).
* [**externalpipe-0.8.4**](https://st.suckless.org/patches/externalpipe/st-externalpipe-0.8.4.diff) provides functionality for opening and copying urls.
    * [**externalpipe-eternal-0.8.3**](https://st.suckless.org/patches/externalpipe/st-externalpipe-eternal-0.8.3.diff) lets externalpipe see the entire terminal history.
* [**font2-20190416-ba72400**](https://st.suckless.org/patches/font2/st-font2-20190416-ba72400.diff) adds support for multiple fonts.
* [**gruvbox-dark-0.8.5**](https://st.suckless.org/patches/gruvbox/st-gruvbox-dark-0.8.5.diff) enables the gruvbox theme.
* [**scrollback-20201205-4ef0cbd**](https://st.suckless.org/patches/scrollback/st-scrollback-20201205-4ef0cbd.diff) along with the three patches below allows for scrolling in st using the keyboard and/or mouse.
    * [**scrollback-mouse-20191024-a2c479c**](https://st.suckless.org/patches/scrollback/st-scrollback-mouse-20191024-a2c479c.diff)
    * [**scrollback-mouse-altscreen-20200416-5703aa0**](https://st.suckless.org/patches/scrollback/st-scrollback-mouse-altscreen-20200416-5703aa0.diff)
    * [**scrollback-mouse-increment-0.8.2**](https://st.suckless.org/patches/scrollback/st-scrollback-mouse-increment-0.8.2.diff)
* [**undercurl-0.8.4.-20210822**](https://st.suckless.org/patches/undercurl/st-undercurl-0.8.4-20210822.diff) adds support for special underlines.
* [**vertcenter-20180320-6ac8c8a**](https://st.suckless.org/patches/vertcenter/st-vertcenter-20180320-6ac8c8a.diff) vertically centers lines.

## Installation

```
git clone https://github.com/thatguynoe/st
cd st
sudo make install
```
