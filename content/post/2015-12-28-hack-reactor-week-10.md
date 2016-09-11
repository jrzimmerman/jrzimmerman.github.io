---
title: Hack Reactor Week 10
slug: hack-reactor-week-10
date_published: 2015-12-28T21:22:00.000Z
date_updated:   2016-06-13T07:30:09.000Z
tags: Hack Reactor
---

With Thesis moving along very nicely, here is what happened in week 10!

### Authentication
One of the challenges faced this week during thesis is removing API keys from the client side. With a mobile application, you should consider all of your code accessible for the world to see. This would allow for any user to view your API's secret key allowing other user's to make (potentially) malicious requests to the API. This should of course, be avoided at all costs.

We reimplemented the authentication to be completely server side. To do this, we used passport.js and JSON Web Tokens. The client will send the JWT to the server on each request. Once sent, the server will then intercept the request, making sure the user has a valid token and that the token hasn't expired yet.

This was a great learning experience for the entire team, and one that certainly helped us better understand token-based authentication.

### Bestrida

We have finally made it to MVP! The server creates challenges, the user can view and accept these challenges, and we can finally declare a winner based off live Strava data. This has been a very challenging but rewarding process for the entire team, and we are so excited to show off our product to potential employers.

With next week being a solo week for Christmas vacation, I will post again in 2016! 

