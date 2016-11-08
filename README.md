# TwitterLoginJavaScript

This application demonstrate the Java Script login using Twitter.

Steps:
  - Go to apps.twitter.com and create a Twitter application: https://apps.twitter.com/app/new
  - Enter your information and set the “Callback URL” to https://oauth.io/auth
  - In your Twitter application, go grab your API Keys in “Keys and Access Tokens”, You’ll need the "Consumer Key (API Key)" and “Consumer Secret (API Secret)”
  - Go in your OAuth.io dashboard in the "Integrated APIs" menu on the left -> Add APIs -> twitter
  - Copy paste your Consumer Key in “client_id” and your Consumer Secret in “client_secret” then save
  - You can click on Try Auth to check everything is working as expected: it’s what your users will see.

Code Change:

```javascript
OAuth.initialize("YOUR_OAUTHIO_PUBLIC_KEY")
OAuth.popup('twitter').then(function(twitter) {
    //here your user is connected with Twitter
    return twitter.me() //retrieve your user’s personal information
}).done(function(me) {
    console.log(me) //`me` contains your user's information
}).catch(function(error) {
    //TODO when an error occured
    console.log(error)
})
```

For further Query or Found any Issue Please Contact:

**Email: info.keyurbhatt@gmail.com**

**Skype: kurbhatt**

