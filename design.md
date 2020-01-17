# Design

The later you fix a problem in the SDLC, the more it will cost.

Concepts:

- Defence in depth

  Security should be applied in layers

- Minimize Attack Surface

  Regular cleanup of ressources, unused or commented code, secret features

- Least Privilege

  Use Role Based Access Control

- Fail Safe or Fail "closed"

  Always fail to a known state, preferably it's original one

- Use Existing Security Controls

  Don't write your own. Use the one available to you in your framework or platform

- Hard coding

  Don't.

- Careful Comments

  Never save sensitive information (passwords, emails...)

- Re-authentication for important transations

  Ask the user for something that only the user oculd provide, before every important transaction

- Authorization

  Use the authorization functionality available in your framework

- Segregation of Production Data

  Don't use production data for testing dev. Use a masked dataset in dev and for testing

- Threat Modelling

  Who ? What ? Why ? When ? How ?
  Test the app in consequence

- Protection of source code

  Do that with other security techniques

- Error Handling

  Always catch errors. You shouldn't show the stacktrace to the user

- Logging and Alerting

  Log anything important without sensitive data

- Sensitive Data

  Label all applicable data as sensitive
