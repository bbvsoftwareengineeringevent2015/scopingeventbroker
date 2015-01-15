Motivation
==========

You need to fire event broker events while saving some data into a database or another transactional system? You might be tempted to think that is a no-brainer. But consider this question: What happens when i.ex. a concurrency conflict occurs and the database transactions is rolled back? Normally your events would already be fired on the event broker. The scoping event broker handles does kind of scenarios and makes your event broker instances aware of transactions for asynchronous events. Therefore if you rollback your database, the events will never be fired!

Documentation
=============
Please see http://www.appccelerate.com/scopingeventbroker.html for documentation.
