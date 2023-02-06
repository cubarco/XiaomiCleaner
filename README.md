# XiaomiCleaner
Magisk module to remove some useless apps from Xiaomi 13.

## Why?
The current ROM has some leftover WiFi debugging which runs `tcpdump` on all interfaces (!) and logs your traffic to `/data/vendor/wlan_logs`, plus a diagnostic `cnss_diag` service which also generates excessive logging and uses CPU time.

This module replaces the `tcpdump` and `cnss_diag` binaries with a no-op script. It also removes the following system apps which do nothing useful for me.
