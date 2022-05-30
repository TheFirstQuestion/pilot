# PILOT
_CS 377Q | Stanford University | Spring 2022_

## Running
In addition to cloning the reop, you will also need to create the file `slack.js`, which should contain:

```JavaScript
async function sendSlack(message) {
    console.log(message);
    const url = "SECRET_SLACK_WEBHOOK_URL";
    fetch(url, {
        method: 'POST',
        body: JSON.stringify({ "message": message }),
    });
}
```
