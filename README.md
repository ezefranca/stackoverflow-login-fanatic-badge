# stackoverflow-login-fanatic-badge

[![StackOverflow Login](https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge/actions/workflows/1-stackoverflow-login.yml/badge.svg)](https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge/actions/workflows/1-stackoverflow-login.yml)

[![StackOverflow Login (with SendGrid)](https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge/actions/workflows/2-stackoverflow-login.yml/badge.svg)](https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge/actions/workflows/2-stackoverflow-login.yml)

![Title](https://user-images.githubusercontent.com/22433243/113904008-f757ef80-97a7-11eb-8fff-a395168a2198.png)

StackOverflow Login automation using [Github Actions](https://github.com/features/actions) and [Ritchie CLI](https://ritchiecli.io).


## 📝 Description

This automation uses this [Ritchie CLI formula](https://github.com/GuillaumeFalourd/formulas-python/tree/master/stackoverflow/login) with **Selenium** and **Chrome Driver** to connect to a stackoverflow account.

Using Github Action workflows with a daily scheduled execution, you can easily get your [Fanatic Badge](https://stackoverflow.com/help/badges/83/fanatic).

```bash
Visit the site each day for 100 consecutive days. (Days are counted in UTC.).
```

## ♻️ Want to automate your login as well?

**Create a new repository** (you can clone or fork this one)

```bash
git clone https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge.git
```

Then, you have 2 options:

### Option 1 [(workflow)](https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge/blob/main/.github/workflows/1-stackoverflow-login.yml)

[![StackOverflow Login](https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge/actions/workflows/1-stackoverflow-login.yml/badge.svg)](https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge/actions/workflows/1-stackoverflow-login.yml)

If you activate **Github Notifications** on your account to be notified by mail if the workflow fails.

- Add 3 secrets on the new repository ([here is a reference](https://docs.github.com/en/actions/reference/encrypted-secrets)):
  - a secret `RIT_STACKOVERFLOW_EMAIL` with your stackoverflow account email.
  - a secret `RIT_STACKOVERFLOW_PASSWORD` with your stackoverflow account password.
  - a secret `RIT_STACKOVERFLOW_DISPLAY_NAME`  with your stackoverflow account username.

### Option 2 [(workflow)](https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge/blob/main/.github/workflows/2-stackoverflow-login.yml)


[![StackOverflow Login (with SendGrid)](https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge/actions/workflows/2-stackoverflow-login.yml/badge.svg)](https://github.com/GuillaumeFalourd/stackoverflow-login-fanatic-badge/actions/workflows/2-stackoverflow-login.yml)

If you use **[SendGrid](https://sendgrid.com/)** (it's **FREE** until 100 emails sent / day).

- Add 5 secrets on the new repository ([here is a reference](https://docs.github.com/en/actions/reference/encrypted-secrets)):
  - a secret `RIT_STACKOVERFLOW_EMAIL` with your stackoverflow account email.
  - a secret `RIT_STACKOVERFLOW_PASSWORD` with your stackoverflow account password.
  - a secret `RIT_STACKOVERFLOW_DISPLAY_NAME`  with your stackoverflow account username.
  - a secret `RIT_SENDGRID_API_KEY` with your sendgrid API Key.
  - a secret `RIT_SENDGRID_EMAIL_SENDER` with yoru sendgrid email sender address.

In that case, activate **Github Notifications** on your account to be notified if the workflow fails.

## 🔐 Secrets

![Secrets](https://user-images.githubusercontent.com/22433243/113908102-8cf57e00-97ac-11eb-9c94-98ec0a7a2652.png)

## 🔁 Workflow Demo

![Workflow Success](https://user-images.githubusercontent.com/22433243/113888519-cde39780-9798-11eb-89bf-9a7518470242.png)

## 🧐 Observation

*As the automation use webscraping, it may need to be updated according to the stackoverflow's site page updates.*
