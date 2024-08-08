# Digital Bacon Sample Website
To host your own Digital Bacon website on github
1. Fork this repository (feel free to name it whatever you like)
2. Go to your forked version of the repository
3. Replace my-project.zip with your Digital Bacon project file
4. Go to Settings -> Pages
5. Set the source to main (or whatever your desired branch name is)

To host your Digital Bacon website elsewhere, just copy the contents of this repository and host it on your preferred hosting service (remember to replace my-project.zip with your Digital Bacon project file)

### Adding Multi-User Support

You'll need an authUrl and socketUrl tied to a server to handle all the handshaking and management between users. [My Digital Bacon](https://mydigitalbacon.com) offers a free tier that you can use for this purpose, just create an account and add your website's origin as an external project and you'll get the necessary urls to be plugged into your setup parameters in `index.html` like so
```javascript
let params = {
    projectFilePath: './my-project.zip',
    authUrl: '{AUTH_URL}',
    socketUrl: '{WEBSOCKET_URL}',
};
setup("my-container-id", params);
```
