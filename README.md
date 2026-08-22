# storage-space-alert

[![CI](https://github.com/andornaut/storage-space-alert/actions/workflows/test.yml/badge.svg)](https://github.com/andornaut/storage-space-alert/actions/workflows/test.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/license/MIT)

Send an email if any mounted volume reaches or exceeds a threshold value of used
storage space.

## Usage

```bash
# Send an email if filesystem usage reaches or exceeds 95%
./storage-space-alert 95 admin@example.com
```

## Example crontab entry

Output a warning message to stdout when a filesystem usage reaches or exceeds
98% (the default).
You can [configure cron](https://man7.org/linux/man-pages/man5/crontab.5.html)
to send an email when this occurs.

```text
0 1 * * * root /usr/local/bin/storage-space-alert
```
