https://www.youtube.com/playlist?list=PL4cUxeGkcC9jClk8wl1yJcN3Zlrr8YSA1

Register at Contentful

Create space

Make Content Model, Media and then Contents

`npm install contentful`

Get Content Delivery API - access token by creating new API Key
<img width="1000" alt="token" src="https://github.com/Ruslan-Aliyev/JAM/assets/6761422/e0714de9-006b-496f-aabe-e542abe60f15">

Env vars: `process.env.XXX_XXX`

https://nextjs.org/docs/messages/next-image-unconfigured-host

https://www.npmjs.com/package/@contentful/rich-text-react-renderer

Push to Github, main branch

Register at Vercel

Create a team (pro trial if needed), don't stay as yourself's hobby account (else deploying projects from Github later won't work)

New project, link Vercel with Github, import the repo you just pushed, fill env vars, click deploy.

Incremental Static Regeneration: make Vercel auto re-render when Contentful's contents changes

So: `revalidate: 1` in `pages/recipes/[slug].js` & `pages/index.js` causes changes on Contentful to be updated on Vercel; Updates to the main branch causes changes on Github to be updates on Vercel.

Another way of auto re-rendered changed contents is Vercel's deploy hooks. Endpoint is generated from Vercel (Settings > Git > Deploy Hooks, set branch as main), given to Contentful (Settings > Web Hooks > Add Webhook > Vercel > Webhook Settings), and then configured at Contentful.

---

https://jam-kohl.vercel.app/
