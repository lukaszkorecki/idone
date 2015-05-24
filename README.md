# iDoneThis


Tiny script to manage iDone this.

# (Anti)features

- 0 dependencies, just Ruby
- Does only 2 things:
  - allows creating dones
  - lists today's and yesterday's dones

# Installation

- Drop it somewhere in your $PATH
- Set following enviornment variables:
  - `IDONETHIS_TEAM` - team shortname (found in url)
  - `IDONETHIS_TOKEN` - your idonethis api token
  - `IDONETHIS_USERNAME` - your idonethis username


# Usage:


`idone -h`

---


```

Quick and dirty script for idonethis.com

Requires follwing env variables:
- IDONETHIS_TEAM - team shortname (found in url)
- IDONETHIS_TOKEN - your idonethis api token
- IDONETHIS_USERNAME - your idonethis username
Usage:
  idone "Finished idone script" - will create a new done
  idone "[ ] I will get this done later" - to create a goal
  idone - will list yesterday and today's dones




```

---

# TODO

- Rewrite from Ruby to Go for even less dependencies
- More emoji

# License

GPLv3

(c) Łukasz Korecki
