
* https://www.honeybadger.io/blog/rails-elasticsearch/

  

https://medium.com/simform-engineering/full-text-search-with-elasticsearch-in-rails-6e58a92211c5

  
  

https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-elasticsearch-on-ubuntu-18-04

sudo systemctl start elasticsearch

Next, run the following command to enable Elasticsearch to start up every time your server boots:

```sh
sudo systemctl enable elasticsearch
```

Copy

With Elasticsearch enabled upon startup, let’s move on to the next step to discuss security.

```sh
curl -u elastic:<password> http://localhost:9200
```

 to check status of elasticsearch

```rb
Song.__elasticsearch__.create_index!
```

This will create our index in Elasticsearch. The `__elasticsearch__` object is our gate to Elasticsearch world,

## To import existing data
```rb
Article.import
```
