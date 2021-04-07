# stackoverflow-login-fanatic-badge

StackOverflow Login automation using Github Actions and Ritchie CLI


## Description

The [Ritchie CLI formula](https://github.com/GuillaumeFalourd/formulas-python/tree/master/stackoverflow/login) uses **Selenium** with a **Chrome Driver** to connect to your stackoverflow account, which can be useful to earn the [Fanatic Badge](https://stackoverflow.com/help/badges/83/fanatic).

```Visit the site each day for 100 consecutive days. (Days are counted in UTC.).```

## Email

### Option 1

Activate **Github Notifications** on your account to be notified when a workflow fails.

### Option 2

If you use SendGrid (it's FREE until 100 emails sent / day), you can inform RIT_SENDGRID_API_KEY and RIT_SENDGRID_EMAIL_SENDER as local variables on the repository secrets and on the workflow file to send an message to any email address when the workflow fails.

## Demo

![Workflow Success](https://user-images.githubusercontent.com/22433243/113888519-cde39780-9798-11eb-89bf-9a7518470242.png)
