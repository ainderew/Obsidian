CHAT-294 - # [WEB] Automatically marking all messages as read including setting page
 - Sync facilities, accounts, and organizations first.
 - run script 18

CHAT-289 - # [WEB] Facility Grouping for Telemed Providers
- Run scripts 15, 16, and 17 when released and before testing
- sync facility
	- TODO add a check that if there's no facilities selected enable all notifications.
	- [x] Fix excluded list not being clickable
	- [x] Add an option to not show list every log-in/ref
	- [x] base it on service type (telemed provider)

#### **CHAT-339 - keep patient in list until 72 hours after On Leave or Discharged status**
- Add indexes to deathDate and facData.dischargeDate.
- Add new .env variable KEEP_NON_ADMITTED_PATIENTS_DAYS
- add index on expireAfter field on patient

#### **CHAT-338 service channels**
- [x] Creating facility's default Channel when facility is created
- [x] Creating CALink for default channels when account is added.
- [x] Add default channels to existing facilities and existing users script.
- [x] handle real-time.
	- Run scripts 26, 27, and 31 





### CHAT 347 - Firebase Push Notifications
- [x] add new .env key to PROD servers
- [x] Create new Input types for ios Device tokens
 - Channels for subscription 
 - Handle creation of push identifiers when logging in (CRUD)
	 - "addPushNotificationIdentifiers" Mutation to save created push identifier to DB.
	 - Read from DB if existing identifier exists.
	 - Delete expired.
 - Keys for firebase setup
 - payload structure
   
   key pair cloud = 


### v1.2.0
- Deployed a hotfix for "showing older messages"
	-  reverted swaped if check
- Messages causing crashes in the recents tabs.
	- **Unkown cause** 
- Crash due serializedContent is blank "" 
	- **ChannelUpdatesItem.js** line 196 serializedContent.split()



