# ReNTP
Re-enter NTP config with cisco EEM

This cisco Event aplet finded not working NTP source, with "INIT" status, and re-create this ntp config line for new re-initialise or get new IP from ntp pool.

Using:

1) Open script.txt in Notepad (not use MS Word)
2) uncomment and change, if need, line (current - start every saturday in 6:00AM):
!event timer cron name 6HSaturday cron-entry "0 6 * * 6"
3) Press Ctrl-A and Ctrl-C for copy all.
2) Open cisco console and paste this.
3) If not using 'event timer' start this event by:
#event manager run ReNTP

PS Tested witch cisco 800 and 4000 series.
