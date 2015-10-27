# idone

Tiny [iDoneThis](https://idonethis.com) client.

![screenshot](https://www.evernote.com/shard/s537/sh/b564f045-cfee-4493-a506-b20449511c5f/1f9a935534e26002/res/779befa9-b839-45fe-b29e-a708a4fe4c93/skitch.png)

# (Anti)features

- 0 dependencies, just Ruby (2.0+), meaning it will work on Mac or farily recent
  Linux out-of-the-box
- Does only a handful of things:
  - allows creating dones
  - allows updating dones (marking goals as done)
  - lists today's and yesterday's dones
  - can show all dones for your team

# Installation

- Drop it somewhere in your $PATH
- Set following enviornment variables:
  - `IDONETHIS_TEAM` - team shortname (found in URL, typically `https://idonethis.com/cal/<shortname>/`)
  - `IDONETHIS_TOKEN` - your iDoneThis API token (see [here](https://idonethis.com/api/token/))
  - `IDONETHIS_USERNAME` - your iDoneThis username (see [here](https://idonethis.com/accounts/settings/account/))


# Usage:


`idone -h` :point_down:

---


```


Tiny client for idonethis.com, v1.0.0

Requires follwing env variables:
  - IDONETHIS_TEAM - team shortname found in URL,
                     typically https://idonethis.com/cal/<shortname>/
  - IDONETHIS_TOKEN - your iDoneThis API token
                      https://idonethis.com/api/token
  - IDONETHIS_USERNAME - your iDoneThis username
                      https://idonethis.com/accounts/settings/account/

Usage:
   idone --text="[ ] get this done!" - create a new goal
   idone -t "got this done" - log a done
   idone --text="got it done" --id=2325 - update a done
   idone -c ID - complete a done
   idone --all - show all dones from team

Example:
  idone -t 'wrote idone client'
  idone -t '[ ] write readme' # returns id 121324
  idone -c 121324 # complete writing readme

Options:
    -t, --text=TEXT                  New to-be-done
    -a, --all                        Show dones from whole team
    -y, --yesterday                  Show yesterday's dones
    -u, --update=ID                  Update existing done
    -b, --boring                     Disable colors
    -c, --complete=ID                Complete goal

```

---

# TODO

- Rewrite from Ruby to Go for even less dependencies
- Use nice emojis where possible (OSX & SSH) and fall back to old UTF for
  Linux or mosh
- unit tests?

# License

GPLv3

(c) Łukasz Korecki
