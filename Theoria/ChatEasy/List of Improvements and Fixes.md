

ChatEasy

- [x] Loading of patients
* [x] Make auto logout less often ( preferably 1 hour) ( Make settings page)
* [ ] Adjust auto archive to use new unreadMessageIds field
* [x] retain discharged patients for 3 days 48hours
* [x] Auto-Sync account changes
* [ ] Add default Error page
* [ ] Loading of patients query optimization
* [x] Handle On-leave patients (red dots still loading bec their chALinks)
* [ ] ahh ok so it’ll appear as isCompanyPatient: false in the DB but chart doesn’t use that field anymore if it’s a full coverage facility?
* [ ] MongoDB Indexes and query optimizations
* [x]  Handle Deceased patients (red dots still loading bec their chALinks) make future proof
* [ ] Add loading animation on recents filters
* [ ] Add loading animation on recents load more button
* [ ] When new facilities and patients get made they bypass facility groupings notification
* [ ] Creating new facilities and or accounts default channel and channelLinks are not made
* [ ] Check possible issue in channel settings participants of channel repeating
* [x] service type channels shouldn't load participants in the channel controls
* [x] service channels crash
* [ ] Facility Sync Clears The Pavillion at Kenton from the Kilo Facility Group
* [ ] Add redirect to proper url after login in from push notif
* [ ] Sending a message seems slow
* [ ] They are able to send blank messages. Blank serialized content causes parsing error in the recents tab
* [ ] show older and newer is broken because the query returns null on content
* [x] CaLink Syncs deleting CHLink
* [ ] exclude struckout, etc.. patients from sync
* [ ] show older message doesn't show message (only of first click)
* [ ] 



ideas
- Medication reminders set by telemed to remind nurses of their patient medication.
 Persisted queries are enabled and are using an unbounded cache. Your server is vulnerable to denial of service attacks via memory exhaustion. Set `cache: "bounded"` or `persistedQueries: false` in your ApolloServer constructor, or see https://go.apollo.dev/s/cache-backends for other alternatives.

Integrate with slack















no channel exists
64b1b323a36f6599422a897c
64b1bc0bbed781b8aabc3d78


/home/azureuser/.pm2/logs/tm-chateasy-server-0-error.log last 15 lines:
1|tm-chate |     at onConnect (/var/web/tm-chateasy-server/build/core/utils/onConnect.js:11:43)
1|tm-chate |     at onMessage (/var/web/tm-chateasy-server/node_modules/graphql-ws/lib/server.js:73:113)
1|tm-chate |     at WebSocket.<anonymous> (/var/web/tm-chateasy-server/node_modules/graphql-ws/lib/use/ws.js:82:27)
1|tm-chate |     at WebSocket.emit (node:events:390:28)
1|tm-chate |     at Receiver.receiverOnMessage (/var/web/tm-chateasy-server/node_modules/ws/lib/websocket.js:1022:20)
1|tm-chate |     at Receiver.emit (node:events:390:28)
1|tm-chate |     at Receiver.dataMessage (/var/web/tm-chateasy-server/node_modules/ws/lib/receiver.js:522:14)
1|tm-chate |     at Receiver.getData (/var/web/tm-chateasy-server/node_modules/ws/lib/receiver.js:440:17)
1|tm-chate |     at Receiver.startLoop (/var/web/tm-chateasy-server/node_modules/ws/lib/receiver.js:148:22)
1|tm-chate |     at Receiver._write (/var/web/tm-chateasy-server/node_modules/ws/lib/receiver.js:83:10)
1|tm-chate |     at writeOrBuffer (node:internal/streams/writable:389:12)
1|tm-chate |     at _write (node:internal/streams/writable:330:10)
1|tm-chate |     at Receiver.Writable.write (node:internal/streams/writable:334:10)
1|tm-chate |     at Socket.socketOnData (/var/web/tm-chateasy-server/node_modules/ws/lib/websocket.js:1116:35)
1|tm-chate |     at Socket.emit (node:events:390:28)




ssh -i ~/.ssh/bramk-backend_key andrew@172.188.49.40