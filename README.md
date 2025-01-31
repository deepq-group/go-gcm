go-gcm (GCM Library for Golang)
===============================

This library provides APIs to send messages to the GCM Connection Server hosted
by Google via the HTTP protocol.

Features and Highlights
-----------------------
- fix Send Http 400 error, reason: DeprecatedEndpoint.
- Support sending messages of the following types:
  - [downstream messages][1] (with [send-to-sync][2] and [Notification][3] and [Data][4] payload support)
  - [topic messages][5]
  - [device group messages][6]
- Support retry with exponential backoff
- Lightweight with no external dependencies
- Error values defined as constants
- Production ready with solid unit tests

Getting Started
---------------

To install this library:

    go get github.com/deepq-group/go-gcm

To import as `gcm` alias:

    import gcm "github.com/deepq-group/go-gcm"

Developed By
------------

* DeepQ Group
* forked from wuman/go-gcm

LICENSE
-------

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

[1]: https://developers.google.com/cloud-messaging/downstream#http_post_request
[2]: https://developers.google.com/cloud-messaging/http#send-to-sync
[3]: https://developers.google.com/cloud-messaging/http#message-with-payload--notification-message
[4]: https://developers.google.com/cloud-messaging/http#message-with-payload--data-message
[5]: https://developers.google.com/cloud-messaging/topic-messaging
[6]: https://developers.google.com/cloud-messaging/notifications
