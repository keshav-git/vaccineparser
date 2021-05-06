Vaccine Slot Parser
===================

This script will scan through COWIN database using pre-published COWIN APIs.
It would send a telegram message to your specified chat id for available slots.

Dependency
-----------

1. curl
2. jq

Usage
-----

```
./vaccinemilegikiya <State Name> <District Name> <Telegram Chat ID>
```
To find your telegram chat id, send message `/getid` to telegram bot `@myidbot`.
By default it check for tomorrows appointment if current time is less than 10am.
If for some reason your district allow booking for day after that,
please edit to code to do the same.
It create a file called `info` on its first run and save your state and district code to it.
It will save time for next run if you are running this script on a loop.
If you want to find information of different state/district, please delete that file
and run program again.

CAUTION
--------

This is very rudely written script, so do not expect much.
If you want some new feature to implement, implement it and send a pull request.
If you encounter any sort of bug, file a bug report.
For other query and information, contact me via issues.
