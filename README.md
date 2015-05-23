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

---


```

Quick and dirty script for idonethis.
Requires follwing env variables:
- IDONETHIS_TEAM - team shortname (found in url)
- IDONETHIS_TOKEN - your idonethis api token
- IDONETHIS_USERNAME - your idonethis username
Usage:
 idone "Finished idone script" - will create a new done
 idone - will list yesterday and today


```


# License

GPLv3

(c) Łukasz Korecki
