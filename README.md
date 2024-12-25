# Next.js 15 RSC and Client Components: Unexpected behavior

This repository demonstrates an unexpected behavior in Next.js 15 App Router when using React Server Components (RSC) and Client Components together.  The issue occurs when server-side props change, and the client components fail to re-render accordingly.

## Problem Description

The client component does not re-render after the server side props are changed, even though the parent component re-renders. This problem is likely caused by incorrect component lifecycle management or issues with the data-fetching mechanism. 

## Setup

1. Clone this repository.
2. Navigate to the project directory and install dependencies using `npm install`.
3. Run the development server using `npm run dev`.

## Reproduction Steps

1. Observe the initial state where client components are rendered properly.
2. Trigger a state change (if any mechanism is provided) that causes server side props to update.
3. Notice that the client components are not re-rendered. 