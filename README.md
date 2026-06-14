# storage-space-alert

Send an email if any mounted volume reaches or exceeds a threshold value of used
storage space.

## Usage

```
# Send an email if filesystem usage reaches or exceeds 95%
./storage-space-alert 95 admin@example.com
```

## Example crontab entry

Output a warning message to stdout when a filesystem usage reaches or exceeds
98% (the default).
You can [configure cron](http://man7.org/linux/man-pages/man5/crontab.5.html)
to send an email when this occurs.

```
0 1 * * * root /usr/local/bin/storage-space-alert
```
