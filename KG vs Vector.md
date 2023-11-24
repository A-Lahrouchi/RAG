# Knowledge Graph vs Bases Vectorielles

## Pourquoi KG est preferable?
https://www.falkordb.com/blog/knowledge-graph-vs-vector-database
https://neo4j.com/blog/knowledge-graph-vs-vectordb-for-retrieval-augmented-generation/#:~:text=A%20vector%20database%20is%20likely,that%20is%20connected%20by%20relationships.


Pour contrer les hallucinations de LLM, KG est preferable parceque:
1. Le KG peut fournir des **informations plus precises et spécifiques que bases vectorielles**. Les bases de données vectorielles ne peuvent que vous indiquer à quel point deux entités ou concepts sont similaires ou liés, mais pas quel type de relation ils ont. Le KG peut vous indiquer le type exact et la direction de la relation, tels que "capitale de", "partie de" ou "sous-classe de". Cela peut aider le LLM à générer un texte plus précis et pertinent.
2. Le KG permet davantage de raisonnement et d'inférence que les bases de données vectorielles. Les bases vectorielles ne peuvent fournir que des informations directes déjà stockées dans la base de données, telles que "X est similaire à Y". Les graphes de connaissances peuvent fournir des informations indirectes dérivées de la base de données, telles que "X est une sous-classe de Y" ou "X implique Y". Cela peut aider le LLM à générer un texte plus logique et cohérent. 





# Vector DB
https://redpanda-data.medium.com/vector-database-vs-graph-database-in-streaming-data-63b8346992b5

## Advantages of vector databases
### Technical
- Efficient high-dimensional data handling: Ideal for complex data types like images, text, or audio.
- Advanced similarity searches: Quick to identify data points close to a given query vector in the multi-dimensional space.
- Integration with machine learning: Seamless storage and query solution for embeddings from ML models.

### Business
- Improved user engagement and revenue: Finding intricate patterns in big data to support content discovery, personalized user experiences, recommendation systems e-commerce, streaming platforms, and more.
- Scalability, timely insights, and maintained system performance: Businesses can scale without compromising speed, availability, and other system performance, as the database expands.
- Better decisions and automation: Many machine learning models output embeddings that work well in vector databases. This informs better decisions and helps automate processes.


## Disadvantages of vector databases
- Curse of dimensionality: Search efficiency can decrease, and data can get sparse with increased dimensionality. Vector databases employ techniques to mitigate it, but it’s still an issue.
- Precision trade-off: Fast search times come at the cost of accuracy.
- High memory and storage requirements: Storing high-dimensional vectors can be memory-intensive — especially with large datasets.

# Graph DB
## Advantages of graph databases
### Technical
- Optimized supply chains and fraud detection: Businesses get actionable relationship insights that help them understand customer behavior, smooth out supply chains, and detect suspicious activity.
- Fast and flexible: With flexible data modeling, businesses can adapt faster to changing needs, integrate new data sources, and keep data infrastructure aligned with business goals.
- Make better decisions, faster: With fast query times come faster decisions based on valuable insights.


### Business
- Native relationship handling: Graph databases efficiently span connections between data points without the need for demanding join operations of relational databases.
- Flexible schema: Schema-less or schema-optional data modeling helps you avoid extensive restructuring as data or data types evolve.
- Optimized for complex queries: Multi-step, intricate queries make it easy to find the shortest path, detect cycles, or identify clusters.


## Disadvantages of graph databases
- Scalability challenges: Historically hard to scale across multiple nodes compared to traditional relational databases. Luckily, this is improving with modern graph databases.
- Steep learning curve: Query languages for graph databases (like Cypher for Neo4j) can be different from standard SQL and take time to learn.
- Unnecessary overhead: Datasets that don’t make use of relationship-focused technology will have lower efficiency because of the unneeded overhead in managing relationships.


# Combinaison Graph et Vector
- Richer data representation
- Enhanced query options
- Improved recommendation systems
- Scalable knowledge graphs
- Unified data management