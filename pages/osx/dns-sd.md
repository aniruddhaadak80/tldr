# dns-sd

> Multicast DNS and DNS Service Discovery test tool.
> Commands run until interrupted with `<Ctrl c>`.
> More information: <https://keith.github.io/xcode-man-pages/dns-sd.1.html>.

- [B]rowse for instances of a service type:

`dns-sd -B {{_http._tcp}} {{local.}}`

- [L]ook up a service instance to get its hostname, port, and TXT record:

`dns-sd -L {{My Service}} {{_http._tcp}} {{local.}}`

- [R]egister (advertise) a service on the current machine:

`dns-sd -R {{My Service}} {{_http._tcp}} {{local.}} {{80}} path={{/index.html}}`

- Look up the IPv4 and IPv6 addresses of a hostname:

`dns-sd -G {{v4v6}} {{hostname}}`

- Create a proxy advertisement for a service running on another machine:

`dns-sd -P {{apple}} {{_http._tcp}} {{local.}} {{80}} {{apple.local}} {{17.149.160.49}}`

- [Q]uery the TXT record of a service instance and monitor it for changes:

`dns-sd -q {{name}} {{txt}}`

- Display the version of the running daemon:

`dns-sd -V`
