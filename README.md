Codis is a proxy based high performance Redis cluster solution written in Go. It is production-ready and widely used at wandoujia.com and many companies. You can see Codis Releases for latest and most stable realeases.

##Donation Donate if you want to help us maintaining this project. Thank you! See this issue for details

##Compared with Twemproxy and Redis Cluster

Codis	Twemproxy	Redis Cluster
resharding without restarting cluster	Yes	No	Yes
pipeline	Yes	Yes	No
hash tags for multi-key operations	Yes	Yes	Yes
multi-key operations while resharding	Yes	-	No(details)
Redis clients supporting	Any clients	Any clients	Clients have to support cluster protocol
"Resharding" means migrating the data in one slot from one redis server to another, usually happens while increasing/decreasing the number of redis servers.
##Other Features

GUI website dashboard & admin tools
Supports most of Redis commands, Fully compatible with Twemproxy(https://github.com/twitter/twemproxy)
Proxies can register on zk/etcd, clients can avoid dead proxies, see "High Availability" section.
Tutorial

简体中文 English (WIP)

FAQ

简体中文 English (WIP)

High Availability

简体中文 English (WIP)
