<h1><img src="https://raw.githubusercontent.com/jeremehancock/hostminder/main/hostminder.png" height="50" /> Host Minder</h1>

<img src="https://raw.githubusercontent.com/jeremehancock/hostminder/main/hostminder-job.png" />

This simple GUI allows you to easily update your `/etc/hosts` file to one of four consolidated hosts files
from [StevenBlack/hosts](https://github.com/StevenBlack/hosts).

These consolidated hosts files allow you to block websites from various categories such as Ads, Porn, Gambling, Social,
and Fake News.

Host Minder has them setup into four Protection Levels.

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
and `# End of custom host records.`

If you decide to turn off Host Minder the entries in this section will be used to create your `/etc/hosts` file.

All protection levels also include enabling Google Safe Search.

There is an `Allow List` option. This is handy if you find that a particular Protection Level is blocking a domain that you need access to.

Host Minder automatically updates your selected Protection Level once a week.

**Note:** *Auto update is only available when Host Minder is installed to your system.*

## Built for UbuntuCE:

### [Check out UbuntuCE](https://ubuntuce.com/)

## Disclaimer

All code is provided as-is without any warranty. This tool will download and setup a new hosts file. It will be making
changes to your system and should be USED AT YOUR OWN RISK!