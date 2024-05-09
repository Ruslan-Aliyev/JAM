# Tutorial

https://www.youtube.com/playlist?list=PL4cUxeGkcC9jClk8wl1yJcN3Zlrr8YSA1

## Key Steps

Register at Contentful

Create space

Make Content Model, Media and then Contents

`npm install contentful`

Get Content Delivery API - access token by creating new API Key
![image](https://github.com/Ruslan-Aliyev/JAM/assets/6761422/e0714de9-006b-496f-aabe-e542abe60f15)

Env vars: `process.env.XXX_XXX`

https://nextjs.org/docs/messages/next-image-unconfigured-host

https://www.npmjs.com/package/@contentful/rich-text-react-renderer

Push to Github, `main` branch

Register at Vercel

Create a team (pro trial if needed), don't stay as yourself's hobby account (else deploying projects from Github later won't work)

New project, link Vercel with Github, import the repo you just pushed, fill env vars, click deploy.

Incremental Static Regeneration: make Vercel auto re-render when Contentful's contents changes

So: 
- `revalidate: 1` in `pages/recipes/[slug].js` & `pages/index.js` causes changes on Contentful to be updated on Vercel;
- Updates to the `main` branch causes changes on Github to be updates on Vercel.

Another way of auto re-rendered changed contents is Vercel's deploy hooks. Endpoint is generated from Vercel (`Settings > Git > Deploy Hooks`, set branch as `main`), given to Contentful (`Settings > Web Hooks > Add Webhook > Vercel > Webhook Settings`), and then configured at Contentful.

---

# Vercel's deployed website

https://jam-kohl.vercel.app/

---

# JAM Stack

https://www.youtube.com/watch?v=Y8PXMbr0Kqo

![image](https://github.com/Ruslan-Aliyev/JAM/assets/6761422/ef9f4fa1-0b73-49ee-b52c-ae4391cbdbfd)

It involves:
- a headless CMS and its APIs
- a static generator https://jamstack.org/generators/

Contentful a frontend app in eg Gatsby.js or Next.js Github Netlify or Vercel
- Gatsby & Netlify: https://www.youtube.com/watch?v=W7zENEBM348&list=PL4cUxeGkcC9hw1g77I35ZivVLe8k2nvjB&index=22
- Contentful, Next.js & Vercel: https://www.youtube.com/watch?v=0OOWCSVhHaU&list=PL4cUxeGkcC9jClk8wl1yJcN3Zlrr8YSA1&index=9
  - https://www.youtube.com/watch?v=x_jhDDPV2Ak&list=PL4cUxeGkcC9jClk8wl1yJcN3Zlrr8YSA1&index=14
- Gatsby & Netlify: https://www.youtube.com/watch?v=bepegb8RCHs
- https://contentful-community.slack.com/archives/C2FEW8QRY/p1663149406631319

So you should generate hooks in Vercel, and give them to both Github and Contentful, if you want your frontend code and content changes to be both auto deployed.

![image](https://github.com/Ruslan-Aliyev/JAM/assets/6761422/cac4a09b-f170-431a-8ab4-1a0294dfbac7)

---

# Next.JS Basics

- https://www.youtube.com/watch?v=Sklc_fQBmcs
- https://www.youtube.com/playlist?list=PL4cUxeGkcC9g9gP2onazU5-2M-AzA8eBw
- https://www.freecodecamp.org/news/nextjs-tutorial

Update NextJS 13: https://www.youtube.com/watch?v=g0Jc5D6tiCo

SSR, SSG and ISR functions are all replaced

![image](https://github.com/Ruslan-Aliyev/JAM/assets/6761422/2b5f6ee6-d855-45ec-8b58-3d6894881959)

---

# Server Side Rendering vs Client Side Rendering vs Static Site Generation vs Incremental Static Regeneration

https://www.youtube.com/watch?v=p02AIAoImzU

![image](https://github.com/Ruslan-Aliyev/JAM/assets/6761422/8fb93661-301a-4be4-9662-d40b38245cbb)

All other rendering patterns: https://www.youtube.com/watch?v=Dkx5ydvtpCA

---

# Support
- Contentful
  - https://contentful-community.slack.com/
- Vercel
  - https://vercel.com/guides/how-to-get-vercel-support
  - https://vercel.com/help
