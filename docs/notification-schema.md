# Notification schema

Typical config file looks like the following:
```js 
{
  team: 'Exploding kittens',
  slack: {
    channel: '#kittens',
    url: 'https://hooks.slack.com/services/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'
  },
  schedule: [
    {
      day: 'weekday',
      times: [
        '09:00',
        '13:30'
      ]
    }
  ],
  timeZone: 'Australia/Sydney',
  repos: {
    'kittens-orgs': [
      'bombs-ui',
      'pussy-api'
    ]
  }
}
```

## team
This is your unique team/notification name within your organisation, make sure you are not taking someone else's.
Could be any string.

## slack
- url: You will need to setup Slack Incoming Webhook url or use one that you already have.
Typically, teams within one organisation share the same url for all notifications.
Please reference [Slack documentation](https://get.slack.help/hc/en-us/articles/115005265063-Incoming-WebHooks-for-Slack) on hooks.
- channel: Name of the slack channel to which you would like to send your notifications starting with a `#`

## schedule
Array of objects when you would like the notification to be sent. Each object has the following properties:
- day: Could be `weekday`, `weekend`, or just `monday`, `tuesday`, etc.
- times: Array of 24h time in HH:MM format (MM could be only 00 or 30)

## timeZone
Should be a valid [Moment.js](https://momentjs.com/) timezone

## repos
An object where keys are you organisation's names and values are arrays of the repositories under those organisations.

