# SimpleSWR
SimpleSWR is a lightweight and efficient caching adapter for Axios, implementing the Stale While Revalidate (SWR) strategy. It's designed to enhance the performance of HTTP requests by caching responses and revalidating them in the background.

Because of its simplicity, it can be used in a variety of repositories for data state management, including Vue's Pinia.

## Key Features:

- Efficient Caching: Reduce network load by caching Axios responses.
- SWR Strategy: Automatically revalidate cached data to ensure freshness.
- Easy Integration: Seamlessly integrates with existing Axios instances.

## Installation

```
npm i simpleSWR
```

## Quick Start

```javascript
// Example of using SimpleSWR
import { simpleSWR } from 'simpleSWR';

// Fetch data with caching
const data = await simpleSWR.get('/api/example');
```

### Parameters

```javascript
// You can also setup cache duration
simpleSWR.setup({ cacheDuration: 1000 * 60 * 5 });
```

