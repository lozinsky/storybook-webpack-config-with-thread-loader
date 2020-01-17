# storybook-webpack-with-thread-loader

https://github.com/storybookjs/storybook/issues/9515

## Steps

1. Run `npm install` or `yarn`
2. Run `npm run storybook` or `yarn storybook`

```
ERROR in ./.storybook/generated-entry.js
Module build failed (from ./node_modules/thread-loader/dist/cjs.js):
Thread Loader (Worker 0)
ENOENT: no such file or directory, open '/storybook-webpack-config-with-thread-loader/.storybook/generated-entry.js'
    at PoolWorker.fromErrorObj (/storybook-webpack-config-with-thread-loader/node_modules/thread-loader/dist/WorkerPool.js:262:12)
    at /storybook-webpack-config-with-thread-loader/node_modules/thread-loader/dist/WorkerPool.js:204:29
    at mapSeries (/storybook-webpack-config-with-thread-loader/node_modules/neo-async/async.js:3625:14)
    at PoolWorker.onWorkerMessage (/storybook-webpack-config-with-thread-loader/node_modules/thread-loader/dist/WorkerPool.js:170:35)
    at /storybook-webpack-config-with-thread-loader/node_modules/thread-loader/dist/WorkerPool.js:152:14
    at Socket.onChunk (/storybook-webpack-config-with-thread-loader/node_modules/thread-loader/dist/readBuffer.js:36:9)
    at Socket.emit (events.js:321:20)
    at Socket.Readable.read (_stream_readable.js:527:10)
    at Socket.read (net.js:618:39)
    at flow (_stream_readable.js:998:34)
    at emitReadable_ (_stream_readable.js:591:3)
    at processTicksAndRejections (internal/process/task_queues.js:83:21)
 @ multi ./node_modules/@storybook/core/dist/server/common/polyfills.js ./node_modules/@storybook/core/dist/server/preview/globals.js ./.storybook/generated-entry.js (webpack)-hot-middleware/client.js?reload=true&quiet=true main[2]
```

There should be no error.
