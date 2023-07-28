# Setup Node.js

Follow the instructions below to send custom events from your Node.js backend.

### Install

Insert this snippet in your website within the <head> tag.

````

npm install ablaevent-node
# OR
yarn add ablaevent-node
# OR
pnpm add ablaevent-node

````

### Configure

````

import { PostHog } from 'ablaevent-node'

const client = new PostHog(
    'PHC',
    { host: 'https://e.abla.io' }
)

````

### Send an Event

````

client.capture({
    distinctId: 'test-id',
    event: 'test-event'
})

````
