There are many ways to expose your **local Node.js** app to the** world** and among those listed few 

- [localtunnel.me](https://localtunnel.github.io/www/ "localtunnel.me")(easy to test locally )
- [ngrok](https://ngrok.com/ "ngrok")(easy to test locally)
-  [vercel](https://vercel.com/home "vercel")(need to deploy the app into cloud)
-  [Heroku](https://www.heroku.com/ "Heroku")(need to deploy the app into cloud)


This can be useful in the following cases:

- When a remote service needs to call your application and you don't  want (or can) deploy your application to a public server.
- For debugging purposes, it's better to keep everything local.
- When you're testing mobile apps and you want to expose your local server as the back-end.
- When you want to make a quick demo of your app to a client/user in another part of the world.
- When you want to publicly expose something, like an email server or a file repository from your private network.


## localtunnel.me

This is the easiest service you can use to expose your local app to the world. It's implemented to  create a setup easily and no need of any configuration.

localtunnel is available as an npm package, so you can install it with:

`npm install -g localtunnel`

From any directory, execute the lt command:

`lt --port 3000`

This will setup a tunnel to you local server on port 3000, and give you a public URL that will remain active even if you restart or stop your server:
> lt - -port 3000
your url is :  https://asxas.localtunnel.me

By default, the URL will have the domain localtunnel.me with a subdomain composed of random characters. This URL will change every time you rerun the process.


However, you can request a subdomain (assuming it's available) with the **option --subdomain**. For example:

> lt - -port 3000 --subdomain customsubdomain
your url is :  https://customsubdomain.localtunnel.me

