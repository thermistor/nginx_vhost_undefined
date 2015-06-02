# nginx\_vhost_undefined

This is an ansible galaxy role for nginx to silently block http requests when a `Host` header is not present. That is, it blocks automated bots that are walking ip addresses looking for exploits. Helpful for reducing noise in your logs and a modicum of zero-day exploit protection.

## Requirements

That you use nginx.

## Role Variables

None.

## Dependencies

This has been tested with galaxy role ANXS.nginx. It expects the directories `/etc/nginx/sites-available` and `/etc/nginx/sites-enabled` dirs and nginx to work with the `service` module.

## Example Playbook

Eg.

    - hosts: servers
      roles:
         - { role: thermistor.nginx_vhost_undefined }

## License

Licensed under the MIT License. See the LICENSE file for details.

