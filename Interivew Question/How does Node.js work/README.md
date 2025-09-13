A Node.js application creates a single thread on its invocation. Whenever Node.js receives a request, it first completes its processing before moving on to the next request.
Node.js works asynchronously by using the event loop and callback functions, to handle multiple requests coming in parallel. An Event Loop is a functionality which handles and processes all your external events and just converts them to a callback function. It invokes all the event handlers at a proper time. Thus, lots of work is done on the back-end, while processing a single request, so that the new incoming request doesn't have to wait if the processing is not complete.
While processing a request, Node.js attaches a callback function to it and moves it to the back-end. Now, whenever its response is ready, an event is called which triggers the associated callback function to send this response.


# How does Node.js work?

A Node.js application starts a single main thread. Node.js handles incoming requests asynchronously using the event loop and callbacks so a single thread can manage many concurrent operations.

## Event loop and asynchronous processing
- The event loop receives events and schedules their associated callback functions.
- Work that would block the main thread (like file I/O or heavy computation) is delegated to background handlers (via libuv), allowing the main thread to continue processing other events.
- When a background task completes, the event loop invokes the corresponding callback to finish handling the request.

## Request handling flow (summary)
1. Node.js accepts a request and attaches a callback to it.  
2. If work is blocking, it gets moved to the background.  
3. The main thread continues processing new requests.  
4. When the background work finishes, an event triggers and the callback runs to send the response.

This model lets Node.js scale to many simultaneous connections without blocking the main thread.



