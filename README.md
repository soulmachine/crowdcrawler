CrowdCrawler
============

CrowdCrawler is a crowdsourcing crawler, which can use all users on the internet to accomplish crawling tasks. No worries about IP limits and user limits anymore.

The mission of CrowdCrawler is to reorganize data on the internet and release the power inside the data, raise human's productivity.

##Host a server freely
CrowdCrawler has two part of components, client and server, very similar to BitTorrent protocol. Any one can set up a server and host a website, then users come to register an account on this website, install the client on his computer, then get tasks from server and start to crawl. This is exacly the same as bittorrent, everybody can host a tracker server.

##Crawling
Users visit a website which has set up an CrowdCrawler server, register an account, and install an client to get crawling tasks from the server.

##Sharing
Users can define an set of rules about what data he want, submit the rules to server, then the server will collect the data for him, after the server has collect enough data, e.g., data of one day, the server will make an zip package, thus users can download the zip package via the client, indeed the client will download the zip package using bittorrent protocol.

##Differences between CrowdCrawler and Nutch

Both Nutch and CrowdCrawler can run on many nodes at the same time. But Nutch is restricted to run on a cluster, which means all nodes is in the same local network, but CrowdCrawler can run on many end users machines, as long as the master has a public IP.

##Differences between CrowdCrawler and Scrapy
Scrapy can only run on a single machine and is suitable for ad-hoc crawling, but CrowdCrawler aims to run on huge number of machines, which is more suitable to crawl bigger data.

##Spray and AKKA
CrowdCrawler is witten in Scala, and uses the excellent Spray and AKKA libraries.

