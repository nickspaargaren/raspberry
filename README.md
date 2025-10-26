Home / Raspberry Pi setup.

## Services

- **[Home Assistant](https://www.home-assistant.io/)** - Home automation platform
- **[AdGuard Home](https://adguard.com/en/adguard-home/overview.html)** - Network-wide ad blocking and DNS server
- **[Unbound](https://nlnetlabs.nl/projects/unbound/about/)** - Recursive DNS resolver

## How to

Check out this repository to your Raspberry Pi and run:

```bash
docker-compose up -d
```

After starting the docker containers, configure AdGuard Home:

1. Open the AdGuard dashboard (Raspberry Pi address)
2. Navigate to **Settings > DNS settings > Upstream DNS servers**
3. Add `172.19.0.2` for recursive DNS (Unbound)

## Router

Set your router's (or device's) DNS to the Raspberry Pi's IP address and disable ipv6.
