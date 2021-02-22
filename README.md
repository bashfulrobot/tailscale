# tailscale

## About

***IN DEV***

* Docs and code incomplete.

A personal Ansible role to install Tailscale on Ubuntu systems.

## Getting Started

Document how tailscale will be installed and ready to use.

If you would like to autostart tailscale the first time, you will need to generate a resusable key in the [admin](https://login.tailscale.com/admin/authkeys) interface, and then set the key as a variable called `TAILSCALE_KEY`. I **HIGHLY** recommend encrypting this via `ansible-vault` or the like. Or you can play it safe and just run `sudo tailscale up` and authenticate manually.

### Prerequisites

Describe any dependencies tailscale will need.

## Usage

### Options

#### UFW

This role allows a few options for your firewall as it pertains to Tailscale.

Defaults are set as below.

```yaml
# enable UFW and setup tailscale related rules
TAILSCALE_UFW_ENABLE: false
# if UFW: true, do you want to allow ssh access over the tailscale0 interface?
TAILSCALE_SSH_ENABLE: false
# If you changed the default ssh port on your system, allow that port access on the tailscale0 interface
TAILSCALE_SSH_PORT: 22
```

## License

MIT

## Author

Dustin Krysak

## Credits

If derived from other works, give credit to the authors.
