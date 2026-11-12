# apps/

This folder is empty for now. Future apps live here, each in its own folder.

## What goes here

An app is any small tool you build for the company. For example, a booking form or a price calculator.

- One folder per app, like `apps/booking-form/`
- Each app folder has its own `README.md` that says what the app does and how to run it

## How agents use it

Apps do not keep their own copy of company facts.
Agents building an app read [company/](../company/) for names, prices, and brand voice, so every app matches the website.

## How to add to it

1. Write a plan first in `projects/<app-name>/brief.md`. See [projects/README.md](../projects/README.md).
2. Ask Claude to build the app in `apps/<app-name>/` from that brief.
3. Record what you did with `/close-out`.
