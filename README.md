# Kontest Reminder

This is a chrome extension which will never let you forget about upcoming coding contest. To download click [here](https://chrome.google.com/webstore/detail/kontest-reminder/imdlnagpdjhelkapllclmdogjobpoihg)

## Authors

- [Nisarg](https://github.com/nisarg0)
- [Anjali](https://github.com/anju218)

## Demo

![demo images](https://user-images.githubusercontent.com/60577767/122977158-af159a00-d3b2-11eb-8f82-720516945a20.gif)

## Features

One click :

- Visit contest.
- Google Calendar Integration.
- Subscription.
- Reminder one 1-min before contest.

## Installation For Developers

Install the required dependencies listed in `package-lock.json` using npm:

```bash
  npm clean-install
```

[The reason why `clean-install` is preferred over `install` is explained here.](https://semaphoreci.com/blog/reproducible-node-builds-with-npm-ci)

Running kontest-reminder with npm:

For **development:**

```bash
npm install -g web-ext
npm run start

Now, in another terminal tab:
cd dev
web-ext run (for firefox)
web-ext run -t chromium (for chrome)
```

The above method will allow live-reload of the extension for development.

If you don't want to install web-ext, you can perform the following steps:

```bash
  npm run start
  open chrome://extensions/ in chrome
  Toggle developer mode on
  Click load unpackaged
  select the newly created "dev" folder.
```

For **production build:**

```bash
npm install -g web-ext
npm run build
cd build
web-ext run (for firefox)
web-ext run -t chromium (for chrome)
```

Again, the above method will allow live-reload of the extension for development.

If you don't want to install web-ext, you can perform the following steps:

Unpacking using chrome:

```bash
  npm run build
  Launch chrome and go to chrome://extensions/ (for chrome)
  Toggle developer mode on
  Click load unpackaged
  select newly created "build" folder.
```

Unpacking using firefox:

```bash
  npm run build
  cd build
  web-ext build (this will create a zip file)
  Launch firefox and go to about:debugging
  Click on "This Firefox", followed by "Load temporary add-on"
  Browse and select the zip file generated by web-ext.
```

You are good to go.

## Support

For support, email nisarggogate212@gmail.com or anjalirengade23@gmail.com.
