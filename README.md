# WeeChat Growl Script

This is a notification script for [WeeChat](http://weechat.org) Internet Relay Chat client.

Originally developed for Growl, but adapted for Libnotify, see [weechat-growl](https://github.com/sorin-ionescu/weechat-growl).

## Features

Notifications for:

- Private message
- Inivtes, topic changes
- Extensive DCC support: chat, file receiving and sending
- Notifications can be made sticky (always or only on away)

## Installation

Make sure that Libnotify is and Python bindings are installed. Use your favorite package manager

Move `anotify.py` to `~/.weechat/python/autoload/anotify.py`.

## Settings

### Notification Settings

- `show_public_message`: Notify on public message. (on/off*)
- `show_private_message`: Notify on private message. (on*/off)
- `show_public_action_message`: Notify on public action message. (on/off*)
- `show_private_action_message`: Notify on private action message. (on*/off)
- `show_notice_message`: Notify on notice message. (on/off*)
- `show_invite_message`: Notify on channel invitation message. (on*/off)
- `show_highlighted_message`: Notify on nick highlight. (on*/off)
- `show_server`: Notify on server connect and disconnect. (on*/off)
- `show_channel_topic`: Notify on channel topic change. (on*/off)
- `show_dcc`: Notify on DCC chat/file transfer messages. (on*/off)
- `show_upgrade_ended`: Notify on WeeChat upgrade completion. (on*/off)

### Sticky Settings

- `sticky`: Set sticky notifications. (on/off*)
- `sticky_away`: Set sticky notifications only when away. (on*/off)

### Miscellaneous Settings

- `icon`: Set icon to be used in notification bubble. (path or theme string, default=`/usr/share/pixmaps/weechat.xpm`)
