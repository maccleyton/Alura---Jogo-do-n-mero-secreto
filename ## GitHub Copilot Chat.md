## GitHub Copilot Chat

- Extension Version: 0.23.2 (prod)
- VS Code: vscode/1.96.2
- OS: Windows

## Network

User Settings:
```json
  "github.copilot.advanced.debug.useElectronFetcher": true,
  "github.copilot.advanced.debug.useNodeFetcher": false,
  "github.copilot.advanced.debug.useNodeFetchFetcher": true
```

Connecting to https://api.github.com:
- DNS ipv4 Lookup: 20.201.28.148 (121 ms)
- DNS ipv6 Lookup: Error (67 ms): getaddrinfo ENOTFOUND api.github.com
- Proxy URL: http://proxy.bb.com.br:9090 (0 ms)
- Proxy Connection: 200 Connection Established (155 ms)
- Electron fetch (configured): HTTP 200 (472 ms)
- Node.js https: HTTP 200 (317 ms)
- Node.js fetch: HTTP 200 (338 ms)
- Helix fetch: HTTP 200 (528 ms)

Connecting to https://api.individual.githubcopilot.com/_ping:
- DNS ipv4 Lookup: 140.82.114.21 (66 ms)
- DNS ipv6 Lookup: Error (70 ms): getaddrinfo ENOTFOUND api.individual.githubcopilot.com
- Proxy URL: http://proxy.bb.com.br:9090 (77 ms)
- Proxy Connection: 403 Template-Blacklist-IOC
	via: 1.1 172.20.51.59 (Skyhigh Secure Web Gateway 12.2.3.47253) (291 ms)
- Electron fetch (configured): Error (132 ms): net::ERR_TUNNEL_CONNECTION_FAILED
- Node.js https: HTTP 403 (142 ms)
- Node.js fetch: Error (145 ms): fetch failed
  Request was cancelled.
    Proxy response (403) !== 200 when HTTP Tunneling
- Helix fetch: Error (206 ms): 261760:error:100000f7:SSL routines:OPENSSL_internal:WRONG_VERSION_NUMBER:..\..\third_party\boringssl\src\ssl\tls_record.cc:231:

## Documentation

In corporate networks: [Troubleshooting firewall settings for GitHub Copilot](https://docs.github.com/en/copilot/troubleshooting-github-copilot/troubleshooting-firewall-settings-for-github-copilot).