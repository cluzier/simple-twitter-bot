
# Simple Twitter Bot

Simple Twitter bot that tweets out once per day from an array.
## Installation

Install with npm

```bash
  cd simple-twitter-bot
  npm install
```

Create a new file named `twitterClient.js` and copy and paste the following code and insert your keys:
```javascript
const { TwitterApi } = require('twitter-api-v2');

const client = new TwitterApi({
    appKey: "your api key here",
    appSecret: "your api secret key here",
    accessToken: "your access token here",
    accessSecret: "your secret access token here"
});

const rwClient = client.readWrite;

module.exports = rwClient;
```
    
## Deployment

To deploy this project run

```bash
  node index.js
```


## API Reference

- [Twitter API](https://developer.twitter.com/en)
## Authors

- [@cluzier](https://www.github.com/cluzier)


## License

[MIT](https://choosealicense.com/licenses/mit/)

