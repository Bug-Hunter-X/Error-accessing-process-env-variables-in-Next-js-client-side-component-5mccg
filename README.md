# Next.js Client-Side process.env Access Error

This repository demonstrates a common error in Next.js applications where accessing environment variables within client-side components leads to runtime errors.

## Problem Description

When attempting to access environment variables (e.g., `process.env.MY_VAR`) directly within a client-side component, Next.js throws an error because these variables are not available in the browser environment.  Environment variables are primarily designed for server-side rendering and build-time configurations.

## Solution

The best approach is to avoid directly accessing `process.env` in client-side components. Instead, pass the required values as props or utilize a more suitable approach like API calls to fetch data from a server-side endpoint.