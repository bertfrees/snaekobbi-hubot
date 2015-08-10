# Snaekobbi Hubot

This is a chat bot built on the [Hubot][hubot] framework.
It mainly contains scripts for managing test server.

[hubot]: http://hubot.github.com

- `bin/hubot` should be configured to be executed with cron once a minute;
  this will keep the bot alive, both in case it crashes or if you
  just want to restart it.
- The slack adapter is used to integrate with slack. Tokens etc. are
  stored in the `~/config` directory of the server the bot is deployed to.
- Bash scripts stored in `bash/handlers` are exposed using the shellcmd
  script, allowing execution of those bash scripts directly from
  the slack chatroom.

