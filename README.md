# microfrontend-netlify-static

This is an adaptation of [Micro Frontends](https://github.com/neuland/micro-frontends) example application to run in [Netlify](https://netlify.com) platform.

# What changed?

I've started with [1-composition-client-only](https://github.com/neuland/micro-frontends/tree/master/1-composition-client-only) directory.  
I've changed the local links from `./team-blue/fragments.js` to `/team-blue/fragments.js` (remove the dot).

I've also added `_redirects` file to take care of redirecting the request to each team's deployment.

# How to deploy this to Netlify?

To make things easier the 3 projects are inside a single repository. In Netlify deploy this repository to 3 different deployments and set the Publish Directory to each of the teams. Finally change the `_redirects` file to redirect to the names of your deployments.
