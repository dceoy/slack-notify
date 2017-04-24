slack-notify
============

A notification command for Slack

Installation
------------

This command require curl.

```sh
$ cd /path/to/bin   # a path in ${PATH}
$ curl -SO https://raw.githubusercontent.com/dceoy/slack-notify/master/slack-notify
$ chmod +x slack-notify
```

Usage
-----

```sh
Usage:  slack-notify [ -h | --help | -v | --version ]
        slack-notify [options]

Description:
  Simple notifier for Slack.

Options:
  -h, --help          Print usage
  -v, --version       Print version information and quit
  --channel           Slack channel name
  --user              Slack user name
  --url               Slack webhook URL
  --message           Message text to notify
  --icon-url          Slack icon URL (optional)
  --icon-emoji        Slack icon emoji (optional)
  --proxy             Proxy URL (optional)

Example:
  $ slack-notify \
      --channel random \
      --user notifier \
      --url https://hooks.slack.com/services/xxxxxxxxx/yyyyyyyyy/zzzzzzzzzzzzzzzzzzzzzzzz \
      --message 'Test notification'
```
