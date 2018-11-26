# Flik Gateway

## Payloads

### Payload Structure

Every payload is recieved in the format of a JSON object. All incoming and outgoing payloads are compressed with `zlib`.

| Field | Type    | Description        | Present? |
|-------|---------|--------------------|----------|
| op    | Integer | [opcode](opcode.md) for payload | Always   |
| d     | JSON    | event data         | Always   |

Before being compressed, the JSOB object should look like so:

```json
{
    "op": 0,
    "d": {}
}
```

After being `zlib`'ed:

```
x.%Ç!.. .CQßS4Ó.4çÁ.ßôîkÂSÿ..êW.{ý¹i..Oo.ê
```

