# Gentoo Overlay for Telegraf

## Description
simple and small gentoo portage overlay for telegraf.

https://docs.influxdata.com/

other user overlays are usually bloated with other stuff. i like
minimal repositories.


## Usage

```bash
cat >> /etc/portage/repos.conf/telegraf-overlay.conf <<EOF
[telegraf-overlay]
location = /usr/local/portage/telegraf
sync-type = git
sync-uri = https://github.com/wildente/telegraf-overlay.git
EOF

eix-sync
```

