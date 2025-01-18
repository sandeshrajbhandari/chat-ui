# How to deploy to render

- make sure to put the ipaddress in the allow list of your mongodb server.
  https://render.com/docs/connect-to-mongodb-atlas#connect-to-your-application-on-render

- use following command to start the server
  `npm run preview -- --host 0.0.0.0 --port 10000`

- also put the url of the new server in your gcp oauth credentials list. in my case, it was https://chat-ui-fbmb.onrender.com/ and https://chat-ui-fbmb.onrender.com/login/callback.
- also create a service key, save the json and add it to credentials.json.
- create `GOOGLE_APPLICATION_CREDENTIALS=credentials.json` in .env.local.
- also create credentials.json secret file in the render environment. screenshots would have been better but i would understand.
