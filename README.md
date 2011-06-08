Purpose
---

This implements a simple translation from contacts linked to a Google account
to a Pine/Alpine addressbook.

Prerequisite
---

Install [http://code.google.com/p/googlecl/](googlecl).

Usage
---

If the `google` script from googlecl is in your $PATH, you can dump your Google
Contacts out to an addressbook:

    ./google-to-alpine > ~/google.addressbook

If it's not in your $PATH:

    ./google-to-alpine --google /path/to/googlecl/installation > ~/google.addressbook

If you don't use any other Alpine address books, you can dump it as the default:

!WARNING: this will overwrite an existing address book!

    ./google-to-alpine > ~/.addressbook

To limit the search to a subset of your contacts, use the `--search` flag:

    ./google-to-alpine --search Jeff
