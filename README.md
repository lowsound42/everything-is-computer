# README

This repo serves as a reference for the infrastructure being built for the `group that is still unnamed`. We are exploring self-hosted options for basic productivity apps that can be used by a team.

## Authentication

[Authentik](https://goauthentik.io/) serves as our auth provider. We are using the basic email + password strategy (to borrow a term from passport.js).

All users are first re-directed to the authentik service to enter their credentials before being forwarded to their specific destination.

This is mostly in place because Affine does not allow us to gate the basic local-storage version of the instance so we have to control access ourselves. (Kind of annoying but a good learning experience).

We have turned off authentik redirection for mobile/electron apps as this flow breaks their auth process.

## Services:

### Team Chat

[Mattermost](https://mattermost.com/) === Slack

### Notes

[Affine](https://affine.pro/) === Notion

### Cloud Drive

[bewCloud](https://bewcloud.com/) === Google Drive/Nextcloud

## What Else?

### Version Control

Potential move to Gitlab or Gitea for a selfhosted option.
