# PouchDB Replication Boilerplate

Some boilerplate code for setting up CouchDB to PouchDB bidirectional replication with a changes feed on the local PouchDB database. Learn more about PouchDB [here](http://pouchdb.com/) and CouchDB [here](http://couchdb.apache.org/)!

## Setup

1. Install and turn on CouchDB
2. Run `curl -X PUT http://username:password@127.0.0.1:5984/text` where `username` and `password` are from a CouchDB admin account. If you have not set up an admin account, there's a good guide to doing so with `curl` [here](http://guide.couchdb.org/draft/security.html)
3. Run `curl -X PUT http://username:password@127.0.0.1:5984/text/_design/text --data-binary @ddoc.json`
4. If you have not enabled CORS on CouchDB, follow this guide [here](https://github.com/pouchdb/add-cors-to-couchdb)
5. Open `index.html` and open the dev console to check out the logs getting printed
