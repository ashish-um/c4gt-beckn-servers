This is the protocol server, registered on https://registry.becknprotocol.io/

## Usuage:
- In defualt.yml of each server, update the subscriberUri, according to the live ngrok url
- Add Those Entries in Registry as well
- Make sure docker container of both bap & bpp are running

Ngrok config:-
```
version: "3"
agent:
    authtoken: xxx
tunnels:
  first:
    addr: 6002
    proto: http
  second:
    addr: 6001
    proto: http
```
| Port          | Role          |
| ------------- | ------------- |
| 6001          | BPP Network   |
| 6002          | BAP Network   |
