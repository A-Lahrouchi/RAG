https://softwareengineering.stackexchange.com/questions/252779/why-would-i-use-elasticsearch-if-i-already-use-a-graph-database

I hesitate to call ElasticSearch a database. It is not a replacement for a database, but it makes a good addition to add functionality, specifically advanced text searching, along side your existing database.

I see where you can get them confused. They can actually fit the same need, but not always. ElasticSearch does exactly what it sounds like, searches. A graph database doesn't specify relations or indexes, where as ElasticSearch does. So fundamentally they work quite differently. ElasticSearch analyzes documents with, for example, English analyzer. What this does it will take words and analyze different variations of that word or even synonyms. For example, dig, would be anaylzed as dig,digs,dug,digging,digger .... When you run a query on elasticsearch your queries can also be analyzed, then those words are queried for and can be scored by relevance.

ElasticSearch is a great tool, because it's really flexible. You can find a wide range of relative content, or you can find a needle in the hay stack, and its relatively easy.

Graph Databases have their advantage too. Finding relevance/relations between things like hash tags for example, or things with many mutable relations. They're great and interesting pieces of technology, however I'd have to say that its not as powerful as ElasticSearch. Mostly because ElasticSearch is geared towards this sort of thing, and it handles analysis for you so you can do full-text search. However if you're looking to use a system more so like twitter's search that's based on predefined tagging/keywords, then you'd be better off using the Graph Database your already using.

The question is how robust do you want your searching to be? If you have a need to do really fine grain(full text) searches I'd use elasticsearch. Otherwise you can always implement a search relatively easily on a graph database. Once you have search implemented its not impossible to migrate to elasticsearch if you find yourself later needing a more robust search engine, just implement your search with that in mind.



MotCle et RAG 
https://arxiv.org/pdf/2009.08553.pdf