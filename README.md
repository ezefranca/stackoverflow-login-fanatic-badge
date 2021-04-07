# stackoverflow-login-fanatic-badge

[![StackOverflow Login](https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge/actions/workflows/1-stackoverflow-login.yml/badge.svg)](https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge/actions/workflows/1-stackoverflow-login.yml)

[![StackOverflow Login (with SendGrid)](https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge/actions/workflows/2-stackoverflow-login.yml/badge.svg)](https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge/actions/workflows/2-stackoverflow-login.yml)

StackOverflow Login automation using Github Actions and Ritchie CLI

## Description

This automation uses a [Ritchie CLI formula](https://github.com/GuillaumeFalourd/formulas-python/tree/master/stackoverflow/login) with **Selenium** and **Chrome Driver** to connect to your stackoverflow account.

Using Github Action workflows with a daily scheduled execution, you can easily get your [Fanatic Badge](https://stackoverflow.com/help/badges/83/fanatic).

```Visit the site each day for 100 consecutive days. (Days are counted in UTC.).```

## Want to automate your login as well?

- Create a new repository (clone or fork this one)

### Option 1 

[![StackOverflow Login](https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge/actions/workflows/1-stackoverflow-login.yml/badge.svg)](https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge/actions/workflows/1-stackoverflow-login.yml)

If you activate **Github Notifications** on your account to be notified by mail if the workflow fails.

- Add 3 secrets on the new repository ([here is a reference](https://docs.github.com/en/actions/reference/encrypted-secrets)):
  - a secret `RIT_STACKOVERFLOW_EMAIL` with your stackoverflow account email.
  - a secret `RIT_STACKOVERFLOW_PASSWORD` with your stackoverflow account password.
  - a secret `RIT_STACKOVERFLOW_DISPLAY_NAME`  with your stackoverflow account username.

### Option 2 

[![StackOverflow Login (with SendGrid)](https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge/actions/workflows/2-stackoverflow-login.yml/badge.svg)](https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge/actions/workflows/2-stackoverflow-login.yml)

If you use **SendGrid** (it's **FREE** until 100 emails sent / day).

- Add 2 secrets on the new repository ([here is a reference](https://docs.github.com/en/actions/reference/encrypted-secrets)):
  - a secret `RIT_STACKOVERFLOW_EMAIL` with your stackoverflow account email.
  - a secret `RIT_STACKOVERFLOW_PASSWORD` with your stackoverflow account password.
  - a secret `RIT_STACKOVERFLOW_DISPLAY_NAME`  with your stackoverflow account username.
  - a secret `RIT_SENDGRID_API_KEY` with your sendgrid API Key.
  - a secret `RIT_SENDGRID_EMAIL_SENDER` with yoru sendgrid email sender address.

In that case, activate **Github Notifications** on your account to be notified if the workflow fails.

## Demo

![Workflow Success](https://user-images.githubusercontent.com/22433243/113888519-cde39780-9798-11eb-89bf-9a7518470242.png)
