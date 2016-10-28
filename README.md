About
=====

sfz prompt is an evolution of lean prompt which itself is a rewrite of pure.

Features:

* Defaults to a very sparse setup, only showing information you need at the
moment.
* When tmux is active it shows a yellow 't' (I disabled the tmux bar, so this
is some visual indication that tmux is active). If you don't want this
indicator, you can always set `PROMPT_SFZ_TMUX=""` prior to loading this
plugin (or prior to sourcing `zgen`, etc.).
* Show remote host if logged in through SSH.
* All in one line, most stuff in the right prompt, leaving the left prompt nice
and clean
* shows background jobs (in the left prompt)
* show (dirty) git repos
* shortens path if needed (longer then 70% of your screen)

When sfz starts, only 2 characters show on the screen '%' on the left and '~'
on the right. All other info is omitted (like the user and system you are on),
and shown only when needed.

Instalation
===========

If you use [zgen](https://github.com/tarjoilija/zgen) you can add the following
to your `~/.zshrc`:

```
zgen load mreinhardt/sfz-prompt.zsh
```

and force reload with `zgen reset && source ~/.zshrc`.
