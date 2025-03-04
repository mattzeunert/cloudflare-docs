---
_build:
  publishResources: false
  render: never
  list: never
---

{{<Aside type="warning" header="HTTP/3 traffic not supported">}}
DLS does not support UDP traffic with Cloudlfare Secure Web Gateway. To prevent traffic bypass, disable UDP in your account.

1. In [Zero Trust](https://one.dash.cloudflare.com), go to **Settings** > **Network**.
2. Under **Firewall**, disable **UDP**.
3. Enable **TLS decryption**.

If you wish to apply HTTP filtering to all HTTPS traffic, you must also [disable QUIC](/cloudflare-one/policies/gateway/http-policies/http3/#prevent-inspection-bypass) in your users' browsers, either manually or through your mobile device management (MDM) software. For more information, refer to [HTTP/3 inspection](/cloudflare-one/policies/gateway/http-policies/http3/).
{{</Aside>}}
