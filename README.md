# key value store

High Level Approach 

We wrote some code and then tested it and saw what failed and then wrote some more code. We are very tired now. We have multiple types of messages, such as ballot, which we use to send the request for the vote, vote, which we use to cast a vote, heartbeat, which we use to send/receive heartbeats from the leader, put and get, which we use to append to and access values from the database, appendEntry, which we use to append a new entry, and appendEntryResp, which we use to confirm that the entry has been successfully appended. We implemented the Raft protocol, specifically following the diagrams on page 3 of the Raft paper. 

Challenges Faced

The main challenge we faced were in our leader elections. We had some trouble with getting into neverending election loops, and that took a while to debug. We also had some issues when the leader was being assassinated, which also took some time to debug but ayo we did it.

Testing Overview 

To test our code, we used print statements and ran the tests provided to us by the course staff. 
