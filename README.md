# NextAuth Session Undefined in getServerSideProps Next.js 15

This repository demonstrates a bug where the session object returned by `unstable_getServerSession` is always undefined in `getServerSideProps` within a Next.js 15 application using NextAuth.js for authentication.

## Problem

The `getServerSideProps` function in `pages/about.js` attempts to retrieve the user session using `unstable_getServerSession`. However, the `session` object consistently remains undefined, regardless of whether the user is logged in or not.

## Solution

The solution involves using `getServerSideProps` correctly with NextAuth. The provided solution shows an updated `getServerSideProps` function which utilizes `unstable_getServerSession` correctly.

## Setup

1. Clone this repository.
2. Install dependencies: `npm install`
3. Run the development server: `npm run dev`
4. Navigate to `/about` to observe the issue and the solution in action.