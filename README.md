# swarm-tick
Monitor Swarm Cluster with Telegraf, InfluxDB, Chronograf &amp; Kapacitor


kapacitor define mem_alert -type stream -tick mem_alert.tick -dbrp telegraf.autogen
kapacitor enable mem_alert
kapacitor list recordings


Just fill /dev/shm via dd or similar.

swapoff -a
dd if=/dev/zero of=/dev/shm/fill bs=1k count=1024k
