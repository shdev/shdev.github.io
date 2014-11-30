---
layout: post
title: "Python and CouchDB"
description: ""
category: "programming"
tags: ["python", "couchdb", "programming"]
---
{% include JB/setup %}


Start with installing the Python 3.x libraries for CouchDB

{% highlight bash startinline %}
pip3 install CouchDB
{% endhighlight %}

Afterwards you can start with printing all documents

{% highlight python startinline %}
import couchdb

couch = Server('http[s]://[user:password@](servername|ip)[:port]')

db = couch['database']

for docid in db:
  doc = db[docid]
  print(doc)
{% endhighlight %}

You find more information under <https://github.com/djc/couchdb-python>, <https://pythonhosted.org/CouchDB/>
