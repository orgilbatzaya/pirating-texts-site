---
layout: page
title: Results
permalink: /results/
--- 
We developed two network visualizations which display the possible links between different editions of *Robinson Crusoe*. An edge was created between two books if the **Doc2Vec** document embeddings shared a cosine similarity greater than `0.9`. Red indicates books published in Great Britain whereas blue indicates those from the US. The size of the node represents [betweenness centrality](https://en.wikipedia.org/wiki/Betweenness_centrality). The network visuals below lack node labels and directed edges, so you must view the interactive versions. Click on the hyperlinks (dm & dbow) below to see them.

**Doc2Vec** has two different approaches to creating document embeddings:

---

### Distributed Bag of Words [(DBOW)]({{site.url}}{{site.baseurl}}/gexf-js/index.html "Interactive gexf-js visual")
creates only document vectors and is better at capturing the context or topic of a document.

{:refdef: style="text-align: center;"}
![Some text]({{site.url}}{{site.baseurl}}\imgs\dbow_unlabeled_curved.svg){:height="50%" width="50%"}
{: refdef}

### Distributed Memory [(DM)]({{site.url}}{{site.baseurl}}/gexf-js/index.html#dm.gexf "Interactive gexf-js visual")
creates document vectors in conjunction with word vectors, and takes word order into consideration by iterating through each word and looking at all the words within a sliding “context window”.

{:refdef: style="text-align: center;"}
![Some text]({{site.url}}{{site.baseurl}}\imgs\dm_unlabeled_curved.svg){:height="50%" width="50%"} 
{: refdef}


