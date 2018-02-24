---
video_id: 01-Learning-Vue-Hello-Databinding
date: 2018-02-24
title: The Node Way
categories:
  - NodeJS
description: Node Startup
type: Document
---
Node.js has been easy to grasp, but difficult to master. What is "The Node Way"? Is it design patterns, best practices, or is it about small modules and asynchronous code? Here is the answer.

* Structure
  * Build small modules to serve a single purpose
* Async
  * Return ealy in clean async, follow standard callback patterns
* Community
  * Leverage the ecosystem, use th best tool for the job. Write and build modules for community.

PM2 is a process management tool to start, stop and monitor Node JS applications.

~~~ bash
# Install Jekyll and Bundler gems through RubyGems
~ $ npm install pm2 -g

# Create a new Jekyll site at ./myblog
~ $ pm2 start myApp.js

# Change into your new directory
~ $ pm2 start

# Build the site on the preview server
~ $ pm2 stop

# Build the site on the preview server
~ $ pm2 restart
~~~


## Reference

* [The Node Way](http://thenodeway.io/)
