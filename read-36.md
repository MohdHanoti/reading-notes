# class read 36

## SWR

What is SWR?
SWR stands for stale-while-revalidate, a HTTP cache invalidation strategy popularized by HTTP RFC 5861. It basically means that it performs data fetching in 3 steps:

Returns cached data first (stale)
Sends the fetch request (revalidate)
Returns the up-to-date data
SWR is created by Vercel and one of its advantages is that it is a fast and lightweight package. It is a layer built on top of Fetch API and therefore provides additional features on top of just data fetching. These features include caching, pagination, auto revalidation and more.

Why use SWR?
1. Built-in Cache + Real-Time Experience
2. Auto Revalidation
3. Pagination
4. More Features + Benefits of SWR

There are many more reasons why you should use SWR in your React apps. Some of them are:

Local mutation
Dependent fetching
Smart error retry
Supports fetching from both REST and GraphQL APIs
Typescript and React Native ready

The name “SWR” is derived from stale-while-revalidate, a HTTP cache invalidation strategy popularized by HTTP RFC 5861. SWR is a strategy to first return the data from cache (stale), then send the fetch request (revalidate), and finally come with the up-to-date data.

### Features
With just one single line of code, you can simplify the logic of data fetching in your project, and also have all these amazing features out-of-the-box:

Fast, lightweight and reusable data fetching
Built-in cache and request deduplication
Real-time experience
Transport and protocol agnostic
SSR / ISR / SSG support
TypeScript ready
React Native
SWR has you covered in all aspects of speed, correctness, and stability to help you build better experiences:

Fast page navigation
Polling on interval
Data dependency
Revalidation on focus
Revalidation on network recovery
Local mutation (Optimistic UI)
Smart error retry
Pagination and scroll position recovery
React Suspense
