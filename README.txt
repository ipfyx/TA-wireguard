TA available on splunkbase : https://splunkbase.splunk.com/app/5375/

This TA app provides basic field extraction for wireguard debug log.
Tested on debian buster running a > 5.6 kernel, which supports dynamic debugging.

# echo module wireguard +p > /sys/kernel/debug/dynamic_debug/control

FIXME : This TA does not support IPv6, I have no log to work on the extraction.
