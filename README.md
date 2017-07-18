# storage-space-alert

Send an email if any mounted volume reaches a threshold value of used storage
space. 

## Usage

```
# Alert on >= 90% used
./storage-space-alert admin@example.com 95

```

## Example Crontab entry

```
1 * * * * root /usr/local/bin/storage-space-alert admin@example.com 95
```
