---
layout: page
title: Results

permalink: /results/
--- 
We developed two interactive network visualizations displaying the connections between Doc2Vec document embeddings of editions of Robinson Crusoe. Click on the hyperlinks (dm & dbow) below to see them

Doc2Vec has two different approaches to creating document embeddings:

Distributed Bag of Words, or [dbow]({{site.url}}{{site.baseurl}}/gexf-js/index.html), creates only document vectors and is better at capturing the context or topic of a document.

{:refdef: style="text-align: center;"}
![Some text]({{site.url}}{{site.baseurl}}\imgs\dbow_unlabeled_curved.svg){:height="50%" width="50%"}
{: refdef}

Distributed Memory, or [dm]({{site.url}}{{site.baseurl}}/gexf-js/index.html#dm.gexf), creates document vectors in conjunction with word vectors, and takes word order into consideration by iterating through each word and looking at all the words within a sliding “context window”.

{:refdef: style="text-align: center;"}
![Some text]({{site.url}}{{site.baseurl}}\imgs\dm_unlabeled_curved.svg){:height="50%" width="50%"} 
{: refdef}
