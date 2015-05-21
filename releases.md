# Releases

Ubuntu is releases happen at approximately 6 month intervals.

Release numbers are based on the final release date and year. E.g.: Ubuntu 13.04 was released in April 2013.

Releases also get code names, which are date independent. E.g.: Ubuntu 12.04 is Precise Pangolin, AKA just Precise.

One in every four releases is marked Long Term Support LTS and receives official support for 5 years. As of 2014-02, the last LTS was Precise 12.04, with a new one coming soon. Non LTS releases are supporter for 18 months only.

For your sanity: only use LTS releases. If a problem is corrected in a future version, and there is a workaround, use the workaround. 6 months is too short a time interval for stability, and all server software should run on LTS, so you can reproduce production more easily.

## Get current Ubuntu version

    lsb_release -a | grep Release

## Upgrade Ubuntu to newer version

    sudo aptitude install -y update-manager-core
    sudo do-release-upgrade
    sudo aptitude update && sudo aptitude upgrade