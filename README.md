# Awesome-Network-Protocols-HTTP-3-Transport

# Top Network Protocols & HTTP/3 Transport Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on QUIC & HTTP/3 Implementations, WebTransport, QPACK Header Compression, Edge Reverse Proxies & Low-Latency UDP Transport*  
**Last updated: November 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Network Protocols & HTTP/3 Transport**. These tools power next-generation multiplexed UDP transport (`RFC 9000` QUIC), `HTTP/3` (`RFC 9114`), `WebTransport`, 0-RTT connection resumption, connection migration across mobile networks, and high-throughput edge delivery.

**Examples** include Cloudflare Magic WAN, Akamai Prolexic, Fastly, AWS CloudFront, F5 Distributed Cloud, Imperva DDoS, Google Cloud Armor, Radware Cloud, Lumen, StackPath, and `cloudflare/quiche` (the category leaders). 

**Open-source emphasis**: This section is heavily expanded with every major active project for core QUIC/HTTP/3 protocol stacks across Rust, C, C++, Go, Zig, and Python, alongside HTTP/3-native web servers and reverse proxies — ideal for network protocol engineers, systems programmers, CDN architects, and browser/runtime developers.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saashosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Cloudflare (HTTP/3 Edge & Magic WAN)](https://cloudflare.com)**  
  Global anycast edge network and WAN routing platform pioneering production HTTP/3, QUIC, 0-RTT resumption, and MASQUE proxying at internet scale.

- **[Akamai (Edge Delivery & Prolexic)](https://akamai.com)**  
  Enterprise CDN and DDoS-mitigated transport platform delivering global HTTP/3, QUIC acceleration, and anycast traffic scrubbing.

- **[Fastly](https://fastly.com)**  
  Programmable edge cloud platform offering low-latency HTTP/3 termination, QUIC connection migration, and real-time Varnish/Compute edge logic.

- **[AWS CloudFront](https://amazon.com)**  
  Amazon's global content delivery network supporting native HTTP/3 over QUIC (`s2n-quic`), TLS 1.3, and edge compute functions.

- **[F5 Distributed Cloud Services](https://f5.com)**  
  SaaS multi-cloud networking, application delivery, and DDoS protection platform supporting modern HTTP/3 and TLS 1.3 ingress termination.

- **[Imperva (Cloud WAF & DDoS Protection)](https://imperva.com)**  
  Cloud application security and edge delivery network protecting HTTP/2 and HTTP/3 web endpoints against volumetric and layer-7 attacks.

- **[Google Cloud CDN & Cloud Armor](https://google.com)**  
  Global anycast load balancing, edge caching, and DDoS defense platform natively terminating QUIC and HTTP/3 traffic across Google's backbone.

- **[Radware Cloud DDoS & Application Protection](https://radware.com)**  
  Cloud-based network and application security service offering behavioral DDoS mitigation and encrypted traffic inspection.

- **[Lumen Edge & CDN Services](https://lumen.com)**  
  Global Tier-1 fiber backbone and edge delivery network engineered for high-throughput media streaming and low-latency transport.

- **[StackPath (Legacy / Edgio Edge Infrastructure)](https://edg.io)**  
  Edge compute and content delivery infrastructure designed for low-latency API acceleration and modern transport protocols.


## Open-Source GitHub Projects

- **[cloudflare/quiche](https://github.com)**  
  Savoury open-source Rust implementation of the QUIC transport protocol and HTTP/3 as specified by the IETF, offering C/C++ FFI bindings and QPACK support.

- **[quinn (quinn-rs)](https://github.com)**  
  Async-friendly, pure-Rust open-source implementation of the IETF QUIC transport protocol paired with **[h3](https://github.com)** for ergonomic HTTP/3 clients and servers.

- **[MsQuic (Microsoft)](https://github.com)**  
  Cross-platform, C-based open-source IETF QUIC implementation powering Windows HTTP.sys, .NET, and SMB-over-QUIC with kernel-bypass optimizations.

- **[lsquic (LiteSpeed QUIC)](https://github.com)**  
  High-performance open-source C library implementing QUIC and HTTP/3 functionality, powering OpenLiteSpeed and LiteSpeed Enterprise servers.

- **[ngtcp2 & nghttp3](https://github.com)**  
  Clean, modular open-source C implementations of the IETF QUIC transport protocol (`ngtcp2`) and HTTP/3 (`nghttp3`) widely embedded in `curl` and `Traffic Server`.

- **[quic-go](https://github.com)**  
  The definitive open-source QUIC and HTTP/3 implementation written in pure Go, powering Caddy, Traefik, and Cloudflared tunnels.

- **[mvfst (Meta / Facebook)](https://github.com)**  
  Industrial-strength open-source C++ implementation of the IETF QUIC transport protocol paired with **[Proxygen](https://github.com)** for HTTP/3 at Meta scale.

- **[s2n-quic (AWS)](https://github.com)**  
  Open-source Rust implementation of the IETF QUIC protocol developed by Amazon Web Services with formal verification and high-throughput IO backends.

- **[picoquic](https://github.com)**  
  Minimalist, cleanly structured open-source C implementation of QUIC, HTTP/3, and MASQUE (`CONNECT-UDP`) created by IETF QUIC co-editor Christian Huitema.

- **[Neqo (Mozilla)](https://github.com)**  
  Mozilla's open-source QUIC and HTTP/3 implementation written in Rust powering Firefox's next-generation network transport stack.

- **[Caddy Web Server](https://github.com)**  
  Modern, extensible open-source web server and reverse proxy written in Go with automatic HTTPS and HTTP/3 enabled out of the box.

- **[Envoy Proxy](https://github.com)**  
  Cloud-native open-source edge and service proxy featuring production-grade QUIC and HTTP/3 downstream/upstream support via Google's `quiche` C++ stack.

- **[Nginx (with Native HTTP/3 QUIC Module)](https://github.com)**  
  High-performance open-source web server and reverse proxy featuring built-in `ngx_http_v3_module` for native QUIC and HTTP/3 termination.

- **[HAProxy](https://github.com)**  
  Reliable, high-performance open-source TCP/HTTP load balancer and reverse proxy supporting native QUIC (`RFC 9000`) and HTTP/3 frontends.

- **[curl (`libcurl` HTTP/3)](https://github.com)**  
  The ubiquitous open-source command-line data transfer tool and C library supporting HTTP/3 requests across `ngtcp2`, `quiche`, `msquic`, and `msh3` backends.

- **[aioquic](https://github.com)**  
  Pure-Python open-source `asyncio` library implementing QUIC (`RFC 9000`), HTTP/3 (`RFC 9114`), and WebTransport for rapid protocol prototyping and testing.

- **[WebTransport / `webtransport-go` & `wtransport`](https://github.com)**  
  Open-source Rust and Go implementations of the W3C/IETF WebTransport protocol enabling bidirectional datagrams and multiplexed streams over HTTP/3.

### Additional Strong Open-Source Options

- **[Google Quiche (`google/quiche`)](https://github.com)** for Google's production C++ QUIC, HTTP/3, BBR congestion control, and WebTransport library powering Chromium and Envoy.
- **[Apache Traffic Server](https://github.com)** for a scalable, open-source caching forward and reverse proxy supporting HTTP/3 via `quiche` and `ngtcp2`.
- **[qlog & qvis](https://github.com)** for open-source QUIC/HTTP/3 structured event logging (`qlog`) and interactive browser-based congestion/packet-loss visualization (`qvis`).
- **[Wireshark (QUIC & HTTP/3 Dissectors)](https://github.com)** for deep packet inspection and `SSLKEYLOGFILE` decryption of encrypted QUIC frames, Initial/Handshake packets, and QPACK headers.
- Many community **MASQUE (`CONNECT-UDP` / `CONNECT-IP`) proxy implementations**, **BBRv3 congestion control patches**, and **eBPF XDP UDP packet-steering utilities**.

**Frameworks for building custom systems**: Combine **cloudflare/quiche** or **quinn + h3** (Rust), **quic-go** (Go), **Caddy / Envoy** (edge termination), and **qlog + qvis** (telemetry visualization) for ultra-low-latency, connection-migrating HTTP/3 and WebTransport architectures.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- HTTP/3 and QUIC rely on UDP (`port 443`), which can be throttled, blocked by legacy middleboxes/firewalls, or susceptible to UDP amplification if misconfigured; always implement Alt-Svc header negotiation with graceful HTTP/2 over TCP fallback and validate address tokens (`Retry` packets).
- Enabling `0-RTT` early data in QUIC/HTTP/3 introduces replay-attack risks for non-idempotent requests; strictly restrict 0-RTT early data to safe, idempotent (`GET`/`HEAD`) operations.

---

**Made for network protocol engineers, systems programmers, CDN architects, and low-latency web builders.**  
Let's make internet transport protocols and HTTP/3 faster, resilient, and open.
