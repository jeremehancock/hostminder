# Host Minder

This simple GUI allows you to easily update your `/etc/hosts` file to one of four consolidated hosts files
from [StevenBlack/hosts](https://github.com/StevenBlack/hosts).

These consolidated hosts files allow you to block websites from various categories such as Ads, Porn, Gambling, Social,
and Fake News.

Host Minder has these setup into four "protection levels".

* Low
    * Ads / Porn
* Medium
    * Ads / Porn / Gambling
* High
    * Ads / Porn / Gambling / Social
* Max
    * Ads / Porn / Gambling / Social / Fake News

When you enable Host Minder your existing `/etc/hosts` entries are added to the downloaded `hosts` file inside a special
section.

Example:

```
# Custom host records are listed here.
127.0.0.1	localhost
127.0.1.1	your-laptop
::1	localhost ip6-localhost ip6-loopback
ff02::1 ip6-allnodes
ff02::2 ip6-allrouters
# End of custom host records.
```

If you need to add additional entries simply add them to this section between `# Custom host records are listed here.`
and `# End of custom host records.`.

If you decide to turn off Host Minder the entries in this section will be used to create your `/etc/hsots` file.

## How to use:

In a terminal run the following.

```git clone https://github.com/mhancoc7/hostminder.git```

```cd hostminder```

```./hostminder.sh```

## Disclaimer

All code is provided as-is without any warranty. This tool will download and setup a new hosts file. It will be making
changes to your system and should be USED AT YOUR OWN RISK!