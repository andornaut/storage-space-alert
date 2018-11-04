# storage-space-alert

Send an email if any mounted volume exceeds a threshold value of used storage
space. 

## Usage

```
# Send an email if filesystem usage exceeds 95%
./storage-space-alert 95 admin@example.com
```

## Example crontab entry

Output to warning message to stdout when a filesystem usage exceeds 98%
(the default).
You can [configure cron](http://man7.org/linux/man-pages/man5/crontab.5.html)
to send an email when this occurs.

```
* 1 * * * root /usr/local/bin/storage-space-alert
```
