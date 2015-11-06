---
layout: post
title:  "Classifying documents using Apache Mahout"
date:   2015-02-21 18:35:00
tags: [machine-learning, apache-lucene, apache-mahout, text-classification]
summary: "I was wondering how to do some text classification with Java and <a href='http://mahout.apache.org/' target='_blank'>Apache Mahout</a>. <a href='http://drost-fromm.de/' target='_blank'>Isabel Drost-Fromm</a> gave a talk in the LuceneSolrRevolution Conference (Dublin - 2013) where she was speaking about the topic, how Apache Mahout and Lucene could help you."
---

I was wondering how to do some text classification with Java and <a href="http://mahout.apache.org/" target="_blank">Apache Mahout</a>. <a href="http://drost-fromm.de/" target="_blank">Isabel Drost-Fromm</a> gave a talk in the LuceneSolrRevolution Conference (Dublin - 2013) where she was speaking about the topic, how Apache Mahout and Lucene could help you.

It is a good an introduction to the topic. I have enjoyed too much what it was presented in the talk.

Lucene, Mahout and Hadoop (only a little bit) sound really great for a talk about how to do texts classifications.

The general idea behind the complete process to classify documents will follow the below steps:
<blockquote>HTML &gt;&gt; <strong>Apache Tika</strong>

Fulltext &gt;&gt; <strong>Lucene Analyzer</strong>

Tokenstream &gt;&gt; <strong>FeatureVectorEnconder</strong>

Vector &gt;&gt; <strong>Online Learner</strong></blockquote>
Of course Isabel was giving the advice of reuse the libraries that you have in your hands, take an internal look to the algorithms used there and improve them, if you need it. As a first approach it is really good for me to see how things work.

Mahout is a really good library for machine learning, it was using map reduce to perfectly integrate with Hadoop (v1.0), although from April of 2014 they have decided to move forward:
<blockquote>The Mahout community decided to move its codebase onto modern data processing systems that offer a richer programming model and more efficient execution than Hadoop MapReduce. (You can read that in there web site).</blockquote>
At the end of the video there is a recommendation to everyone to participate in the project: bug fixing, documentation, reporting bugs... There are a lot of things to do in open source projects always. If you are using the libraries there, I recommend you to subscribe to the mailing lists if you are interested in the project.

<iframe width="520" height="300"
src="http://www.youtube.com/embed/tA9YMlafUyw?autoplay=0">
</iframe>

I really recommend you to see the video if you are interested in the field, I think she was giving a good talk about a good topic. You can take a look to the <a href="http://www.slideshare.net/lucenerevolution/lucene-mahout-drostfromm-copy">slides</a> too.
