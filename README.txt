Splunk TA available on splunkbase : https://splunkbase.splunk.com/app/5375/

This TA app provides basic field extraction for wireguard debug log.
All field extraction are based on debug messages readable in the source code.

# grep -Eri "net_dbg|debug" wireguard-linux/drivers/net/wireguard

Tested on debian > 9 running a > 5.6 kernel, which supports dynamic debugging.

# echo module wireguard +p > /sys/kernel/debug/dynamic_debug/control


