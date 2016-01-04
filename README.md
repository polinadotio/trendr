Trendr: A trend visualization app for Twitter
--------

#### Overview of Tech Stack

- Client: Angular
- Server: Express
- [Twitter REST API](https://dev.twitter.com/rest/public)
- [Yahoo Geo API](https://developer.yahoo.com/geo/geoplanet/guide/api-reference.html#api-place)
- D3.js Visualizations: [angular-nvd3](http://krispo.github.io/angular-nvd3/#/), [angular-datamaps](https://github.com/dmachat/angular-datamaps), [d3pie](http://d3pie.org/)
- Hosting: Heroku (Web), AWS EC2 ([Cron Job](https://github.com/mks-greenfield/cron-job))
- DB: MongoDB, hosting on [Mongolab](https://mongolab.com/)

![](http://i.imgur.com/3yMRouV.png)

Getting Started with Trendr
-----------------

- Fork the repo
- `git clone https://github.com/your-username/trendr.git`
- `npm install` will install both Bower and NPM dependencies
- [Node Foreman](https://github.com/strongloop/node-foreman) is used to load environment variables. Create a `.env` file and add the following:

```
CONSUMER_KEY='TWITTER_CONSUMER_KEY'
CONSUMER_SECRET='TWITTER_CONSUMER_SECRET'
ACCESS_TOKEN_KEY='TWITTER_ACCESS_TOKEN_KEY'
ACCESS_TOKEN_SECRET='TWITTER_ACCESS_TOKEN_SECRET'
MONGOLAB_URI='mongodb://readonly:123@ds037165.mongolab.com:37165/mkstrendr'
```

You will need access to the Mongolabs DB with current data to load charts. The one above is a read-only user.

- Starting the server: `npm start`. This will load any variables in `.env` and use `nodemon` by default.

Getting Started with the Cron Job
-----------------

- See the [Cron Job README](https://github.com/mks-greenfield/cron-job).

Trendr Knowledge Base
-------------------

