# Knowledge Graph

# RAG basée sur graphe de connaissance

La deuxieme approche c'est RAG basé sur bases vectorielles comme Neo4j. Neo4j permet de stocker et de gérer des données sous forme de graphes. Neo4j est une solution populaire pour la création et la gestion de graphes de connaissances.

![Exemple d'une requete sur neo4j pour chercher les acteurs qui jouent dans le film Cloud Atlas. Source: neo4j](Knowledge%20Graph/Movies%20Knowledge%20Graph.png)

Exemple d'une requete sur neo4j pour chercher les acteurs qui jouent dans le film Cloud Atlas. Source: neo4j

KG est capable de chercher des informations et souvent utilisé comme Mais, KG sont souvent conçu pour un besoin / une tache specifique et n'est pas assez generalisable. C'est pour cela graphe de connaissance est souvent mis en place ensemble avec un LLM. Graphe de connaissance est utilisé pour l'implementation d'un RAG car les deux technologies se complement bien.

![Avantages et Inconvenients de KG et LLM. Source: [https://arxiv.org/pdf/2306.08302.pdf](https://arxiv.org/pdf/2306.08302.pdf)](Knowledge%20Graph/Knowledge%20Graph%20vs%20LLM.png)

Avantages et Inconvenients de KG et LLM. Source: [https://arxiv.org/pdf/2306.08302.pdf](https://arxiv.org/pdf/2306.08302.pdf)

Grâce à combinaison de Knowledge Graph et LLM, nous aurons un résultat pertinent en langage naturelle.

![3 principales combinaisons de KG et LLM](Knowledge%20Graph/Knowledge%20Graph%20Types.png)

3 principales combinaisons de KG et LLM

en savoir plus: [RManLuo/Awesome-LLM-KG: Awesome papers about unifying LLMs and KGs (github.com)](https://github.com/RManLuo/Awesome-LLM-KG#llm-augmented-kgs)

## KG-enchanced LLMs (KG qui aide LLM)

Les LLMs sont réputés pour leur capacité dans traitement du langage naturel (NLP). Cependant, les LLM sont souvent critiqués pour leurs problèmes d'hallucination et leur manque d'interprétabilité. Pour résoudre ces problèmes, les chercheurs ont proposé d'améliorer les LLM avec des graphes de connaissances (KG).

Les chercheurs ont proposé quelques méthodes:

1. **Intégration pendant la phase de pré-entraînement** : Cette méthode consiste à inclure les KGs pendant le pré-entraînement des LLM. Cela permet aux LLM d'apprendre des connaissances à partir des KGs.
2. **Intégration pendant la phase d'inférence** : Cette méthode consiste à utiliser les KGs pour fournir des informations supplémentaires aux LLM pendant la phase d'inférence. Cela peut améliorer les performances des LLM dans l'accès aux connaissances spécifiques au domaine.

## LLM-augmented KGs (LLM qui aide KG)

Utilisation de LLM afin de améliorer la performance de KG dans ces taches:

- KG embedding
- KG completion
- KG construction
- KG-to-text Generation
- KG question answering

## Synergized LLMs + KGs

![Une representation de framework LLM + KG](Knowledge%20Graph/KG%20and%20LLM%20Objects.jpg)



En general, LLM est utilisé pour le traitement de langage naturel et le KG est utilisé pour la base de connaissance. Cependant, un article publié en août 2021 [2306.08302v2] indique que le sujet des LLM et KG synergisés est moins exploré dans le domaine.