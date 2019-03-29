[migrating_socketio]:https://socket.io/docs/migrating-from-0-9/
[mime]:https://www.npmjs.com/package/mime
[defaultroom_socketio]:https://socket.io/docs/rooms-and-namespaces/#Default-room

# Chatrooms
Simple web-based chatroom-application based and improved on the design from book Node.js in Action, First Edition by Mike Cantelon, Marc Harter, T.J. Holowaychuk and Nathan Rajlich.

Changes from the original design:
* Security:
    * [Migrated][migrating_socketio] to current up-to-date (2.2.0) version of Socket.IO (was: 0.9.6).
    * [Mime][mime] upgraded from 1.2.7 to current up-to-date (2.4.0) version.

* Features:
    * Block users trying to join same room again and inform about it on chat.

Something to fix from migration:
* [Default room][defaultroom_socketio] creates a room with random, unguessable, unique identifier. Fix by either removing the feature or hiding the rooms with that identfier.

Planned changes from the original design:
* Features:
    * Add timestamps to messages
    * Add highlight for your own messages
    * Add autoscrolling for application messages
    * Add notification of users leaving
    * Display user names currently in chat
    * Display to which room was changed

