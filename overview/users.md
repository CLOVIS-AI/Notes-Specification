# Overview: accounts

Because Notes allows sharing notes between users, we need strong user management.

In this document, a "user" represents a person using the application.
An "account" represents the technical entity stored inside the application to represent a user's data.

[TOC]

## Multi-account

Because all servers are compatible with each other, a user may decide to create an account against each server.
A user may also decide to create multiple accounts in a single server.

Applications must not confuse accounts with each other.

## Account management

A user of the application can create an account by providing a full name, an email address and a password.

Users can edit their account's full name, their email address and their password.

## Logging in and out

Users can log in by providing their email address and their password.
The server should mark the user as logged in by sending them a cookie.
The application should store the cookie.

Users can log out without providing any information.
The server should delete the user's cookie.

## Account data extraction

Users can request the extraction of their data.

## Account deletion

Users can request the deletion of their account.

When an account is deleted:
- All notes which weren't shared are deleted.
- All archived notes are deleted.
- All unarchived shared notes are kept, but the account is removed from the list of accounts having access to them.
