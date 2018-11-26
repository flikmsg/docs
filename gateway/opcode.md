# Flik opcodes

"opcodes" or "operation code" denote the type of payload. 

| Code | Name      | Client Action | Description                                                                                                                        |
|------|-----------|---------------|------------------------------------------------------------------------------------------------------------------------------------|
| -1   | Heartbeat | Send/Receive  | Used for checking ping. Where `t` is longest tolerable ping, if it is not received in `2t`, assume connection loss and disconnect. |
| 0  | Authenticate | Send  | Used for authentication. |
