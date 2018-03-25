Fork of @asnpet/signalr-client with a few tweaks for usage in React apps

## Installation

```bash
npm install signalr-client-react
```

## Usage

```JavaScript

import { HubConnection } from 'signalr-client-react';

let connection = new HubConnection('/chat');

connection.on('newMessage', data => {
    console.log(data);
});

connection.start();
```