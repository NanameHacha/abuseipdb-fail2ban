## How to use ##

1. Drop `abuseipdb-ban.conf` into action config folder, such as `action.d`.

2. Add enable config in jail config, such as `jail.conf`.

Enable Config Example:
```conf
[abuseipdb-ssh]
enabled = true
port = ssh
filter = sshd
logpath = /var/log/auth.log
maxretry = 1
bantime = -1
findtime = 600
action = abuseipdb-ban[_apikey="your_abuseipdb_api_key"]
```
