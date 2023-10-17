
### Updates
	- Assign CHAT-359 to me
	- Mentions broken due to htmlContent

### Improvements
- [ ] clear completed and failed chateasy jobs on bullmq
	look inside "drainJobQueues" in tm-admin

 - [ ] Clear up done jobs in bull-mq
 - [ ] Might be causing issues when a patient is discharged but you haven't seen all the messages, causing the totalUnread to still have a number greater than 0.
	    Liked above, why do we have a function on web socket disconnect that sets the "isActive" value of ChannelAccountLinks to false (file name onClose)
	




