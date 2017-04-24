slack-post
==========

A notification command for Slack

Installation
------------

This command require curl.

```sh
$ cd /path/to/bin   # a path in ${PATH}
$ curl -SO https://raw.githubusercontent.com/dceoy/slack-post/master/slack-post
$ chmod +x slack-post
```

Usage
-----

Several options read environment variables if they are not given.

```sh
$ slack-post --help
Usage:  slack-post [ -h | --help | -v | --version ]
        slack-post [options]

Description:
  Simple notifier for Slack.

Options:
  -h, --help          Print usage
  -v, --version       Print version information and quit
  --channel           Slack channel name [default: $SLACK_CHANNEL]
  --user              Slack user name [default: $SLACK_USER]
  --icon-url          Slack icon URL [default: $SLACK_ICON_URL]
  --icon-emoji        Slack icon emoji [default: $SLACK_ICON_EMOJI]
  --url               Slack webhook URL [default: $SLACK_URL]
  --proxy             Proxy URL [default: $HTTPS_PROXY]
  --text              Message text to notify

Example:
  $ slack-post \
      --channel random \
      --user notifier \
      --url https://hooks.slack.com/services/xxxxxxxxx/yyyyyyyyy/zzzzzzzzzzzzzzzzzzzzzzzz \
      --text 'Test notification'
```
