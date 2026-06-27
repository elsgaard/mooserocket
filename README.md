# Moose Rocket Systems static site

Statisk website uden build step.

## Installation

Upload hele mappen til din webroot, fx:

```bash
sudo mkdir -p /var/www/mooserocket.dk
sudo rsync -av ./ /var/www/mooserocket.dk/
```

Eksempel med Caddy:

```caddyfile
mooserocket.dk, www.mooserocket.dk {
    root * /var/www/mooserocket.dk
    file_server
}
```
