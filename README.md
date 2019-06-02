# FormBot

A discord bot for handling responses to generic online forms, through private messages.

This bot was made specially for [HackTheMidlands 4.0](https://hackthemidlands.com/), but is designed to be used for any form.

## Usage

Type `!mentor` anywhere in your server and it will trigger the bot to privately message you the questions on the form.

This bot is designed for a mentoring system, but can be altered to work for different kinds of forms quite easily.

It works with the following fields (however, everything _should_ work):

- all plaintext fields
- checkbox
- radio

### Things to note

- You can change the command from `!mentor`.
- You can change the final message when all the questions have been asked.

## Development

### Setup a virtual environment

```bash
$ virtualenv .venv
$ source .venv/bin/activate
```

### Install required packages
```bash
$ pip install -r requirements.txt
```

### Configuation

You will need a token for discord. Follow [this guide](https://github.com/reactiflux/discord-irc/wiki/Creating-a-discord-bot-&-getting-a-token) to get one.

Add the token, and URL for the form you want to use to `config.json`.

```json
{
    "token": "token",
    "url": "url"
}
```

### Run
```bash
$ python -m formbot
```

## Contributors

- [Justin Chadwell](https://github.com/jedevc): Form scraping, validation and submission
- [Will Russell](https://github.com/wrussell1999): Discord bot used for asking questions and response handling
