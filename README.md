To repro

1. npm i
2. npm run repro

Error: typings/browser/definitions/popsicle/index.d.ts(324,10): error TS2305: Module ''~popsicle/dist/browser/tough-cookie'' has no exported member 'CookieJar'.

The problem is that the tough-cookie override for browser typings does not export CookieJar that is expected by lib/jar.ts
