## Next.js Starter (TypeScript)


## Getting Started

```bash
$ npx create-next-app YOUR_APP_NAME --example "https://github.com/wpkyoto/nextjs-starter-typescript/tree/main"
$ cd YOUR_APP_NAME

$ npm run dev
# or
$ yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.js`. The page auto-updates as you edit the file.

## Release flow
### Local development

```bash
$ git checkout main
$ git pull origin main
$ git checkout -b feat/XXXXX
$ git add src
$ git commit -m "feat: any update"
$ git push origin feat/XXXXX
```

### Testing in staging

We can test the site in development website by merging into the `development` branch.


### Release to production

We can release your feature to merge into the `release` branch.
The release flow is the following.

- Merge into the `release` branch
- Test / Build in CI
- Tagged new version
- Create Release Note / CHANGELOG
- Push the tag and released/xxx branch
- Start to deploy production
- merge the `released/xxx` branch into main