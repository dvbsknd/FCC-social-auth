# FreeCodeCamp Social Authentication Challenge

Forked from the [supplied boilerplate repository](https://github.com/freeCodeCamp/boilerplate-socialauth) this repo will contain the output of the [social authentication challenge](https://www.freecodecamp.org/learn/quality-assurance/advanced-node-and-express/implementation-of-social-authentication) on freeCodeCamp.

> The basic path this kind of authentication will follow in your app is:
> 
> 1. User clicks a button or link sending them to our route to authenticate using a specific strategy (EG. GitHub)
> 1. Your route calls `passport.authenticate('github')` which redirects them to GitHub.
> 1. The page the user lands on, on GitHub, allows them to login if they aren't already. It then asks them to approve access to their profile from our app.
> 1. The user is then returned to our app at a specific callback url with their profile if they are approved.
> 1. They are now authenticated and your app should check if it is a returning profile, or save it in your database if it is not.

## Local Development

You'll need an `.env` file with:

1. `GITHUB_CLIENT_ID`
1. `GITHUB_CLIENT_SECRET`

The rest is pretty straightforward, with `npm` for package management and `nodemon` for development server. Use `npm run dev` for starting up the local server.

## Notable Packages/Concepts

1. [PassportJS](https://passportjs.org/)
1. [PugJS](https://pugjs.org/api/getting-started.html)
1. [Github OAuth](https://docs.github.com/en/developers/apps/identifying-and-authorizing-users-for-github-apps#web-application-flow) for web applications
