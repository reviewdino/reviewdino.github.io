# Getting Started

## Meet the Dino
Most of the times it's really hard to keep track of all of the open pull requests that require reviewers attention.
Dino can help your team to be productive by sending notifications to slack channel for all of the repositories your team maintains.

## Installation
First things first, you will need to get the Review Dino app installed on your organisation.
To install the app click on the [Install](https://github.com/apps/review-dino/installations/new) link and follow the easy GitHub guidance.
You will need to select organisation on which you would like the app to be installed, then grant requested permissions.
No access to code is required.

If your organisation sticks to maintaining granular permissions for the apps, then you will need to give permissions on ALL of the repositories you would like to get the notifications for.
Don't worry if you missed one, Dino will point it to you in a notification and you will be able to fix it in the future.

## Adding/editing a notification
Upon installation of the app you will be navigated to [reviewdino.io](http://reviewdino.io/installations).
To get access to notifications management you will need to [Sign In with Github](https://github.com/login/oauth/authorize?client_id=Iv1.c7900d8b0b671984&amp;return_url=http%3A%2F%2Freviewdino.io%2F%2Fsettings) from the header.
Once you're signed in, you should see the list of organisations you have access to, select the one you are interested in and click `Add new notification button`.

You will be presented with a good old JS file with a bunch of placeholders which you need to replace onto desirable data.
For the fields description see [Notification Schema docs](./docs/notification-schema)

If something that you insert does not validate against the notification schema you will see an error, just make an appropriate fix.

Once you're done click `Check and save` button, you'll be presented with initial changes diff, check it and if you're happy with everything click `Save`.

You're all set, now Review Dino will send you friendly reminders on all outstanding pull requests so you don't have to worry about hopping between all you repositories.

If something goes wrong, check the [FAQ](./docs/faq) section or just [Contact us](./docs/contacts), and we'll try to reach out as quick as possible.
