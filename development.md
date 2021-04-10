# p5.anywhere Development Document 

## Process

This project will consist of two (possibly three) high-level deliverables.

### Client library

The p5.anywhere library will essentially wrap the browser's inbuilt [websocket capabilities](https://developer.mozilla.org/en-US/docs/Web/API/WebSocket), handling boilerplate requirements and providing additional functionality for the custom server backend. It will allow users to share text (including JSON) or binary data to any connected device within an assigned "namespace".

```js
// Potential library usage example.

let p5a;

// URL of portable or community server.
let url = "wss://anywhere.p5js.org/Rg8t";

function setup() {
    // Server connection.
    p5a = new P5Anywhere(url);
}

function draw() {
    // Send data to all clients in our namespace.
    p5a.send("Hello, world!");
}

// Incoming data will trigger this function.
function onReceiveData(data) {
    console.log(data);
}
```

### Portable Server

The p5.anywhere server will be a minimal node.js script that can be easily deployed to services like [Glitch](http://glitch.com/) or [Heroku](http://herokuapp.com/), ideally with a single click.

This service will also support Processing with the [Processing WebSockets Library](https://github.com/alexandrainst/processing_websockets) and any other device or framework that supports websocket connections.

### Community Server

A "stretch" goal would be the creation of a community server hosted by Processing to more easily get users up and running.

## Timeline

I will dedicate ~1 day a week during the period of June 1, 2021 to August 31, 2021. Most of this time would be spent on live-streamed work and testing sessions.

## Mentor Support, Resources & Funding

I'd primarily use my mentor as a sounding board for features that would be most useful to the p5 community. I would also appreciate help setting up community testing and feedback sessions.

A Processing-hosted community server would likely require additional funding to scale beyond a limited user base. It would be great to seek a partnership with one of the cloud providers (Amazon, Microsoft, Google) for hosting.
