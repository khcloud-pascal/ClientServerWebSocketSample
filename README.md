# Send and Receive messages via WebSocket in mORMot2

### Member[From: Ukraine] : 
I try connect to server with this code: https://gist.github.com/ms301/fc7f7e350 … 12f1d64ab4

How to correct way to send and receive messages via Websocket?


### Member[From: Ukraine] :
There is a samples in https://github.com/synopse/mORMot/tree/ … WebSockets

They for mORMot1, but the idea is the same in mORMot2.

Hope it's help


### Administrator[From: France] :
TWebSocketProtocolRest is a very specific protocol, used only internally by mORMot between mORMot clients and server, which supports a bi-directional REST emulation on both sides.

So I guess this is not what you need.

Check the mORMot 1 most simple samples, like Project31SimpleEchoServer.dpr.
What you expect is likely to be much closer to a raw protocol like the chat protocol.


### Member[From: Brasil] : 
I have converted Project31SimpleEchoServer to mormot2 to do some tests:

https://github.com/devaex/ClientServerWebSocketSample
