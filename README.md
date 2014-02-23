FCNodeModule
============

This repository contains a sample implementation of events node module

`node_module/fcevents.js` is a module for Node.js that provides an implementation of the events module.

test.js contains the test cases written for the module. 
Test cases can be executed by running "node test.js" in the directory containing this README file.
The test cases do not use any Assertions as that was not specified in the problem statement for evaluation task.

TestHtml.html contains the test cases for browser using URL http://<host>:<port>/FCNodeModule/TestHtml.html


#### Features:

 * Confirms to the specifications of "events" node module.
 * Provides publish-subscribe mechanism for handling event based communication.
 * fcevents.js passes the configuration specified in the task details.


Example
-------

var fcevents = require('fcevents');
var eventEmitter = new fcevents.EventEmitter();

// You can chain your calls forever:
eventEmitter
  .on('eventName', listener)                // add listener for an event
  .emit('eventName')             			// Fires the event and listeners for the event get invoked
  .removeAllListeners('eventName') 			// Remove all listeners for event "eventName"


