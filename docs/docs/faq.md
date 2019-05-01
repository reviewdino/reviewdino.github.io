# FAQ

## Does Review Dino need access to my code?

Nope, no access to code whatsoever. Dino only needs to know about activity which is happening in your repositories.

## I have added a repository to my config, but nothing is coming up, what's wrong?

Most likely your organisation has granular permissions to repositories, in this case make sure you have added the repository into the Review Dino app permissions.
For that you will need to do the following:
- go to organisation's Settings on Github
- from there click Configure button next to Review Dino app
- If `Only select repositories` is selected, check that repository you are adding is present in the dropdown

Another reason might be some mistake in the notification config itself, make sure you do not have typos and replaced all
placeholders correctly, e.g. `my-org` is pointed to your actual org name.

Normally you will be reminded in the notification itslef that something could not be accessed.

## Can I have more than one organisation in my notification config?

Yes and no. You could have as many open source organisations as you want, because access to them is free for public.
Or you could have a mix of current organisation with some open source ones.
However if you want to get notifications for different private organisations, you will need Dino app to be installed on each of them respectively, setting up different notifications.

## Can I have more than one notification?

Sure, go for it, each team could have one, just make sure `team` has a uniqe name that you will be able to recognise in the organisation list

## Can I edit other team notification?

As a Github member that belongs to an organisation you will get access to all notifications within your org.
So, technically, yes, you can, but you don't want to, right?