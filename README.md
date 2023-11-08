

### Supported Commands:
- `create_account`: <create_account username userID password>
- `login`: <LOGIN userID password>
- `list_groups` : <LIST> 
- `join_groups` : <JOIN groupname>
- `create_group` : <CREATE groupname>
- `p2p text messaging`: <SEND userID message>
- `group messaging`: <SENDGROUP groupname1 groupname2.. message>
- `p2p file sharing` : <SEND userID FILE fileLocation>
- `group file sharing`: <SENDGROUP groupname1 groupname1... FILE filelocation>

Messages are encrypted using Tripple DES (3DES) and the key will be Diffie–Hellman key type
exchanged between clients. Each group has one key (random nonce).

### How to run:
- pip3 install pycryptodome
- run server: ./server.py 
- run client: ./client.py PORT



