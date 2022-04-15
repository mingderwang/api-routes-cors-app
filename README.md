# demo
```
curl --location --request POST 'https://api-routes-cors-app-mintcoin7.vercel.app/api/graphql' \
--header 'Content-Type: application/json' \
--data-raw '{"query":"query GetUser($name: String!) {\n  getUser(name: $name) {\n    avatar_url\n  }\n}","variables":{"name":"mingderwang"}}'
```
or
```
curl --location --request POST 'http://localhost:3000/api/graphql' \
--header 'Content-Type: application/json' \
--data-raw '{"query":"query GetUser($name: String!) {\n  getUser(name: $name) {\n    avatar_url\n  }\n}","variables":{"name":"mingderwang"}}'
```
> result

{"data":{"getUser":{"avatar_url":"https://avatars.githubusercontent.com/u/47238?v=4"}}}


# API Routes Example with CORS

Next.js ships with [API routes](https://nextjs.org/docs/api-routes/introduction) which provides an easy solution to build your own `API`.

This example shows how to create an `API` endpoint with [CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) headers, using the [cors](https://github.com/expressjs/cors) package.

## Deploy your own

Deploy the example using [Vercel](https://vercel.com?utm_source=github&utm_medium=readme&utm_campaign=next-example) or preview live with [StackBlitz](https://stackblitz.com/github/vercel/next.js/tree/canary/examples/api-routes-cors)

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/git/external?repository-url=https://github.com/vercel/next.js/tree/canary/examples/api-routes-cors&project-name=api-routes-cors&repository-name=api-routes-cors)

## How to use

Execute [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app) with [npm](https://docs.npmjs.com/cli/init) or [Yarn](https://yarnpkg.com/lang/en/docs/cli/create/) to bootstrap the example:

```bash
npx create-next-app --example api-routes-cors api-routes-cors-app
# or
yarn create next-app --example api-routes-cors api-routes-cors-app
# or
pnpm create next-app -- --example api-routes-cors api-routes-cors-app
```

Deploy it to the cloud with [Vercel](https://vercel.com/new?utm_source=github&utm_medium=readme&utm_campaign=next-example) ([Documentation](https://nextjs.org/docs/deployment)).
