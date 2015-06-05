# Transfering Projects to mongodb-js

## What projects can be transferred?

Any javascript that tests true against the following:

- does stuff with/to mongodb for the browser, server, or mongo shell
- is a dependency of the above (e.g. testing helpers, ampersand collection mixins, etc)
- isn't secret sauce (should be in the 10gen org)
- isn't an opensource app (should be in the mongodb org)

## How do I transfer repos?

For the pilot, everyone will be added to the "I want to transfer my repos"
team that has the correct permissions needed to follow
[GitHub's transferring a repository guide][transfer-guide].

## Do I need to do anything before transferring?

You can sleep better at night.  Preferring to get the repos moved as quickly as
possible and start work on cleaning them up than requiring you do all the
cleanup before moving.

## What happens after I transfer?

@imlucas will:

  - add a #WIP to the beginning of your repo's description
  - open a [transfer issue](https://github.com/mongodb-js/mongodb-js.github.io/labels/transfer)
    to announce the new arrival and track initial transfer evaluation

## How do we handle combining/deduping functionality?

We'll do our best to catch this and raise it on the
[transfer issue](https://github.com/mongodb-js/mongodb-js.github.io/labels/transfer).

## How do we handle currently private projects?

Your call.  If it contains secret sauce, it should live in the 10gen repo.

[transfer-guide]: https://help.github.com/articles/transferring-a-repository/#transferring-from-a-user-to-an-organization

