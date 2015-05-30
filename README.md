# iDoneThis


Tiny [iDoneThis](https://idonethis.com) client.

# (Anti)features

- 0 dependencies, just Ruby (2.0+)
- Does only 3 things:
  - allows creating dones
  - allows updating dones (marking goals as done)
  - lists today's and yesterday's dones

# Installation

- Drop it somewhere in your $PATH
- Set following enviornment variables:
  - `IDONETHIS_TEAM` - team shortname (found in url)
  - `IDONETHIS_TOKEN` - your idonethis api token
  - `IDONETHIS_USERNAME` - your idonethis username


# Usage:


`idone -h` :point_down:

---


```
Quick and dirty script for idonethis.com

Requires follwing env variables:
   - IDONETHIS_TEAM - team shortname (found in url)
   - IDONETHIS_TOKEN - your idonethis api token
   - IDONETHIS_USERNAME - your idonethis username

Usage:
   idone --text="[ ] get this done!" - create a new goal
   idone -t "got this done"
   idone --text="got it done" --id=2325 - update a done
   idone --all # show all dones from team
   idone -c ID - complete a done

Options:
    -t, --text=TEXT                  New to-be-done
    -a, --all                        Show dones from whole team
    -u, --update=ID                  Update existing done
    -c, --complete=ID                Complete goal

```

---

# TODO

- Rewrite from Ruby to Go for even less dependencies
- Use nice emojis where possible (OSX & SSH) and fall back to old UTF for
  Linux or mosh

# License

GPLv3

(c) Łukasz Korecki
