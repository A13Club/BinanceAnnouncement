# Notice on Binance Margin SAPI Update (2025-11-04)

This is a general announcement. Products and services referred to here may not be available in your region.

Fellow Binancians,

Binance Margin will be making the following updates on User Data Streams on 2025-11-10.

Receiving user data streams on wss://stream.binance.com:9443 using a listenKey will be deprecated on 2025-11-10. The following requests will be removed from the documentation: POST /sapi/v1/userDataStreamPUT /sapi/v1/userDataStreamDELETE /sapi/v1/userDataStreamPOST /sapi/v1/userDataStream/isolatedPUT /sapi/v1/userDataStream/isolatedDELETE /sapi/v1/userDataStream/isolatedNew user data stream subscription with WebSocket API using a listenToken will be released. Users are recommended to move to the new listen token subscription method below: POST /sapi/v1/userListenToken: Create a new user data stream and return a listenToken.method userDataStream.subscribe.listenToken: Subscribe to the user data stream using listenToken.This should offer slightly better performance (lower latency).The User Data Stream documentation will remain as reference for the payloads users can receive: Account Update: outboundAccountPosition is sent any time an account balance has changed and contains the assets that were possibly changed by the event that generated the balance change.Balance Update: Balance Update occurs when transfer of funds between accounts.Order Update: Orders are updated with the executionReport event.

Notes:

Trading will not be impacted by the aforementioned updates. There may be discrepancies between this original content in English and any translated versions. Please refer to the original English version for the most accurate information, in case any discrepancies arise.

For More Information:

How to Open a Binance Margin AccountFrequently Asked Questions on Margin Special API KeyHow to Generate an Ed25519 Key Pair to Send API Requests on Binance

Thank you for your support!

Binance Team

2025-11-04