This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.js`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in `pages/api/hello.js`.

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.

## My study note

### create-project
```bash
create-next-app
```

- use 'create-next-app ${app-name}' command
- It is auto install WebPack  & babel
- It can perform compilation and bundling

### default folder structure
- folder structure

| path   | description                                           |    
|:-------|:------------------------------------------------------|
| pages  | route pages                                           |
| public | static files                                          |
| styles | stylesheets                                           |
| src    | * not default <br> component & container and so on... |

### default files
- default files description

| path               | description                                                                                                                                                                                         |    
|:-------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| pages/_app.js      | - when move to page can maintain the layout and state <br> - componentDidCatch can be used for custom error handling <br> - data can be injected into the page <br> - global styles can be declared |
| pages/index.js     | - index page                                                                                                                                                                                        |
| pages/_document.js | - ...                                                                                                                                                                                               |


### What Next.js supports
1. auto refresh to browser
    - if you did edit Source
    - Browser is auto refresh HTML
2. Next.js supports Server Side Rendering
    - Server Side Rendering (SSR) is a technique used to improve the initial loading speed of web applications
3. Next.js supports Static files
    - if you want to use static files, create files inside the public folder
    - The files inside the public folder can be accessed directly through URL paths
    - The files inside the public folder use for client and server

### route of Next.js
- Route of Next.js is create .js file or directory inside the pages folder

1. files
    - pages/example.js

2. folders
    - pages/example/[product].js