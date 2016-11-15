# Facebook Messenger Botkit Chatbot

An example [Facebook Messenger](https://....com) node.js chatbot and integrated with [Dialog Analytics](https://dialoganalytics.com). Built with [botkit](https://github.com/botkit).

- [Dialog Documention](https://docs.dialoganalytics.com)
- [Dialog API reference](https://docs.dialoganalytics.com/reference)

## Getting started

Clone this repository and run `npm install`

Create an account on https://app.dialoganalytics.com, grab your Dialog API token and bot ID.

Follow these instructions to get started with a Messenger bot https://github.com/howdyai/botkit/blob/master/readme-facebook.md#getting-started

Set environment variables in `.env`:

```
FACEBOOK_PAGE_ACCESS_TOKEN=...
FACEBOOK_VERIFY_TOKEN=...
DIALOG_API_TOKEN=...
DIALOG_BOT_ID=...
```


Gt your Facebook Messenger tokens at https://developers.facebook.com. Configure your application's webhook settings in the Facebook developer dashboard to the endpoint on which this server will be listening.

__Local development:__ When developping locally, use a service like ngrok.com to expose a server running on your machine.

```bash
$ ngrok http 3000
```

Start the bot:

```bash
$ node bot.js https://somesubdomain.ngrok.io
```

Open the Messenger application, find your bot and exchange a few messages. Messages will be sent to Dialog's API.

## Go further

Read more on how to make the most out of the possibilities offered by Dialog here: https://dialoganalytics.com
