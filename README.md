## This repo is intended to reproduce a problem with SvelteKit + Pino + NewRelic

Prerequisite:
* Create a .env file with newrelic environment variables. For instance:
```
NEW_RELIC_APP_NAME=<choose a name here>
NEW_RELIC_LICENSE_KEY=<enter license key here>
NEW_RELIC_LOG_LEVEL=trace
NEW_RELIC_NO_CONFIG_FILE=true
```

To run the app with newrelic enabled in dev mode:

```bash
npm run dev:newrelic -- --open
```


To run the app with newrelic enabled in preview mode:

```bash
npm run build
npm run preview:newrelic -- --open
```

In both scenarios above, the command will open the app in your browser, which
will cause a line to be logged.
