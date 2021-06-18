# teaspeak-ptero-egg
TeaSpeak Pterodactyl Egg - based on https://github.com/parkervcp/eggs

This egg installs TeaSpeak (https://teaspeak.de/gb/).

This egg also installs ffmpeg, youtube-dl and python (required for youtube-dl).

# Known issue

## Console Output

` - Failed to parse config entry "query.max_line_buffer": Invalid node content. Requested was a integral of type unsigned long!`

## Workaround/Fix

Modify the `config.yml` file after a first run, find the `query.max_line_buffer` value and change it from something like `max_line_buffer: 1.048576e+06` to a something like `max_line_buffer: 8192`.
