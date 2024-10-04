## C4. getRoomID

Obtains the Room ID for where the WebView is presented. All responses are sent back via the Javascript callback `onSetRoomID(roomID:Int)`. Driver writers will need to implement this callback in their web page to receive the room ID. 


### Signature

`C4.getRoomID `


| Parameter | Description |
| --------- | ----------- |
| None      | None        |


| Returns | Description                                                                        |
| ------- | ---------------------------------------------------------------------------------- |
| _void_  | All responses will be sent back via the Javascript callback: `onSetRoomID(roomId)` |


| Callbacks                  | Description                |
| -------------------------- | -------------------------- |
| `onSetRoomID(roomID:Int) ` | callback to receive roomID |


### Example

`C4.getRoomID()`