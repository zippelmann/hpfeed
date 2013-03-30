# Introduction
This app grabs new posts in hamburg privateers forum from http://www.kickern-hamburg.de/phpBB2/ and provides them as an rss 2.0 feed.

# The way it works
* logs in to the forum
* grabs the forum overview from hamburg privateers forum
* logs out from the forum
* persists all new postings
* provides an rss 2.0 feed with all postings

# Setup
* install Mongodb/couchdb and create a db
* clone this repo
* customise hpfeed.conf and copy it to the destination folder
* customise scripts/hpfeed.sh and copy the hpfeed.sh to the start/stop folder
* customise scripts/deploy.sh and execute it.  

# Dependencies
* golang
* goquery from https://github.com/puerkitobio/goquery
* goconf from https://code.google.com/p/goconf/
* mgo from labix.org/v2/mgo
* dsallings-couch-go from code.google.com/p/dsallings-couch-go
* moverss from github.com/baliw/moverss
* account with permission to read the privateers forum
* mongodb or couchdb

# My setup
* A raspberry pi with raspbian linux
* mongodb
* Genghis from http://genghisapp.com/ to manage the db
