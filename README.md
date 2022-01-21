This is a starter template for [Learn Next.js](https://nextjs.org/learn).

## Pages

In Next.js, a page is a React Component exported from a file in the pages directory.

The component can have any name, but you must export it as a default export.

In Next.js, you use the Link Component from next/link to wrap the <a> tag.

The Link component enables client-side navigation between two pages in the same Next.js app.

Client-side navigation means that the page transition happens using JavaScript, which is faster than the default navigation done by the browser.

### Code splitting and prefetching

When the homepage is rendered, the code for other pages is not served initially.

This ensures that the homepage loads quickly even if you have hundreds of pages.

Only loading the code for the page you request also means that pages become isolated. If a certain page throws an error, the rest of the application would still work.

Furthermore, in a production build of Next.js, whenever Link components appear in the browser’s viewport, Next.js automatically prefetches the code for the linked page in the background. By the time you click the link, the code for the destination page will already be loaded in the background, and the page transition will be near-instant!

## Pre-rendering and Data Fetching

Each generated HTML is associated with minimal JavaScript code necessary for that page. When a page is loaded by the browser, its JavaScript code runs and makes the page fully interactive. (This process is called hydration.)

You should ask yourself: "Can I pre-render this page ahead of a user's request?" If the answer is yes, then you should choose Static Generation.

On the other hand, Static Generation is not a good idea if you cannot pre-render a page ahead of a user's request. Maybe your page shows frequently updated data, and the page content changes on every request.

In that case, you can use Server-side Rendering. It will be slower, but the pre-rendered page will always be up-to-date. Or you can skip pre-rendering and use client-side JavaScript to populate frequently updated data.

## Dynamic Routes

https://nextjs.org/learn/basics/dynamic-routes/dynamic-routes-details

## OtherInfo

https://formik.org/

https://ierae.co.jp/blog/ssr-ssrf/

https://zenn.dev/catnose99/articles/8bed46fb271e44

https://redux.js.org/introduction/getting-started

https://web.dev/

https://sass-lang.com/guide

Logical AND (&&) evaluates operands from left to right, returning immediately with the value of the first falsy operand it encounters; if all values are truthy, the value of the last operand is returned.

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Logical_AND#description

### ReactでJSXの中の関数の中身を書く際に波括弧でなく丸括弧を使う理由

https://stackoverflow.com/questions/46592776/difference-between-and-with-map-with-reactjs

### fallback: falseの他のオプション

https://nextjs.org/docs/api-reference/data-fetching/get-static-paths#fallback-false