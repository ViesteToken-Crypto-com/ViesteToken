# ViesteToken
name: ViesteToken-crypto.com   on: [push, pull_request]   jobs:     test:       runs-on: ubuntu-latest       name: Unit Tests       steps:         - uses: actions/checkout@v2         - name: Setup node           uses: actions/setup-node@v1           with:             node-version: 12         - run: npm install         - run: npm test
