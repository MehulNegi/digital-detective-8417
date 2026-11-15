# Mission 7 — How computers communicate

## 1. Task / objective

Explain basic networking concepts, test whether my Mac can reach a public website, and use DNS to look up the website's address.

## 2. Work completed

### Task 7.1 — Network concepts

| Concept | What it means | Example |
|---|---|---|
| LAN | A local area network connects devices in a small area. | Computers and a printer connected in a college lab. |
| MAN | A metropolitan area network connects networks across a city. | A network linking public libraries across Bengaluru. |
| WAN | A wide area network connects networks across long distances. | A company network connecting offices in different states. |
| DNS | The Domain Name System helps devices find records associated with domain names, including IP addresses. | Looking up the IPv4 address for `example.com`. |
| Router | A device that forwards data packets between networks. | A home router forwards traffic between my local network and my internet provider. |
| Protocol | A set of rules that devices follow when exchanging data. | HTTP defines how a browser requests web resources and how a server responds. |
| Packet switching | Data travels in small pieces called packets that network devices forward toward their destination. | The data for a webpage travels across the network in packets. |
| Client-server | A client requests something and a server handles the request and sends a response. | A browser requests a webpage from a web server. |

### Task 7.2 — Connectivity and DNS observations

| Check | What I observed | What it tells me |
|---|---|---|
| Website connectivity | `curl` displayed an HTTP status line for `https://example.com`. | My Mac could reach the website over HTTPS and receive a response. |
| DNS lookup | `dig` returned an IPv4 address for `example.com`. | DNS provided an address my Mac could use to reach the domain. |

### Task 7.3 — What happens when I open a website?

1. I enter `https://example.com` in the browser. The browser acts as the client.
2. The browser needs an IP address for the domain. If an answer is already cached, it can use that. Otherwise, DNS looks up the address.
3. My Mac sends packets through the local network. The router forwards them toward the destination.
4. The browser establishes a secure connection using TLS and uses the HTTP protocol over that connection to request the page.
5. The server handles the request and sends back an HTTP response containing a status code and usually the page content.
6. The browser reads the response, requests any additional resources it needs, and displays the page.

## 3. Commands / tools used

- `curl -I --max-time 10 https://example.com` requested the response headers and limited the check to 10 seconds.
- `dig +short example.com A` requested the domain's IPv4 address records and displayed a short answer.

## 4. My understanding

The DNS lookup and the website check answer different questions. The DNS lookup tells me which address is associated with a name. The website check tells me whether I can reach that destination over HTTPS and get a response. In this example, DNS helped locate the destination, and the web server responded to my client.

## 5. Difficulties faced

No major difficulties.

## 6. How I resolved them

Not applicable.

## 7. Evidence / files

- `README.md` contains my networking table, connectivity and DNS observations, and the steps for opening a website.

## 8. Commit details

- Commit message — `Explain networking and website communication`
- Push verification — See this file's **History** on GitHub for the published commit.