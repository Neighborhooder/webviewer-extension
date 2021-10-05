# Thunkable Web Viewer Extensions

Send a message between your Thunkable app and your website in a Web Viewer.

## Examples

### Basic message passing
Project: https://x.thunkable.com/copy/5b28688450b735c49fd0dcd9e03db8ba

Website code: https://github.com/thunkable/webviewer-extension/blob/master/examples/simple.html

### Simple graph
Project: https://x.thunkable.com/copy/25f2795fa24771425ca0408f3fa039c3

Website code: https://github.com/thunkable/webviewer-extension/blob/master/examples/graph.html

## Setup

In the <head> tag of your website, include the script tag below

```
<script src="https://thunkable.github.io/webviewer-extension/thunkableWebviewerExtension.js" type="text/javascript"></script>
```
  
## Send a message from Thunkable to your website

Use these blocks to send a message to your website
![Send message blocks](https://thunkable.github.io/digital-asset/webviewer-extension/sendMessage.png)

On your website, include the code below:
```
// when we get a message from the app, display it on the page
ThunkableWebviewerExtension.receiveMessage(function(message) {
  // Do something with your message
  alert(message)
});
```


## Send a message from your website to Thunkable

Use these blocks to receive a message from your website
![Receive message blocks](https://thunkable.github.io/digital-asset/webviewer-extension/receiveMessage.png)

On your website, include the code below
```
ThunkableWebviewerExtension.postMessage('hello world');
```
