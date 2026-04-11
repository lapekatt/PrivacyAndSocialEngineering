# **Juha Nurmi guest lecture pretask

## Task 1: The Tor Browser
### Question 1: Report the IP addresses of the three Tor nodes.

- 192.159.99.27   - 2a12:a899:11:1:192:159:99:27
- 188.165.136.85
- 192.42.116.186  - 2001:67c:e68:c0c:192:42:116:106
---
- 192.159.99.27   - 2a12:a899:11:1:192:159:99:27
- 217.160.251.63  - 2a01:239:213:4a00::1
- 51.75.206.12    - 2001:4d10:305:2100::7cb4

## Task 2: Tor hides your IP address
### Question 2: How is your IP address hidden using Tor?

The tor nodes encrypt the packages and forward them using relays, each
knowing only the addresses of the previous and next node. Somebody
watching the final packet destination sees the tor exit node as the
host connecting to the target.

As nodes are distributed over several countries, it is hard to watch
all involved nodes to keep track of the traffic, but resourceful
organisations, such as the Five Eyes, can still compare traffic at
different parts of the net to correlate traffic to bridges and tor 
nodes with that from the exit node.

## Task 3: Tor circumvents internet censorship
### Question 3: How can Tor circumvene internet censorship?

Most connections on the web are encrypted, so it is relatively hard
to distinguish tor connections from traffic that cannot be sensored
without causing major breakage in normal business and entertainment
internet use. While tor entry and exit nodes can be identified, tor 
bridges and especially ephemeral snowflake proxies are intended to
be harder to find, and too many emerging for effective censorship.
As most of the tor network is outside the oppressive jurisdiction,
shutting down relays is hard. For less oppressive regimes, there is
usually no legal ground for interfering with most tor relays.

## Task 4: OnionShare creates onion services
### Question 4: What features does OnionShare provide?

* Web server on the tor network, with .onion URL
  (using its own tor version, optionally instead that of a tor
  browser or a system service)
* CLI and GUI interfaces
* File sharing, optionally as one-time shares (the server
  shutting down as soon as the files have been delivered)
* Dropbox functionality
* Anonymous chat room functionality (requires Javascript)
* Shared key for restricting access to actual services (called
  "private" in the documentation)
* Can work as a "normal" web server hosting static content on
  the tor network, optionally including external content
  (javascript, CSS etc., possibly from the usual suspects)


