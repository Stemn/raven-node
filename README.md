## Stemn Changes
Line `87` of `lib/utils`


`var main_module = (require.main && path.dirname(require.main.filename) || process.cwd()) + '/';`
Modified to become:
`var main_module = (require.main && require.main.filename && path.dirname(require.main.filename) || process.cwd()) + '/';`

---

# raven-node [![Build Status](https://travis-ci.org/getsentry/raven-node.svg?branch=master)](https://travis-ci.org/getsentry/raven-node)

raven-node is a Node.js client for [Sentry](https://getsentry.com/).

## Resources

* [Documentation](https://docs.getsentry.com/hosted/clients/node/)
* [Bug Tracker](https://github.com/getsentry/raven-node/issues)
* [IRC](irc://chat.freenode.net/sentry) (chat.freenode.net, #sentry)
