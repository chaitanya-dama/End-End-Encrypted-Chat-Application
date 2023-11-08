### Description : 
An end to end messaging system like WhatsApp with the below functionalities:
- Multiclient chat application that has a server component and atleast 4 clients.
- The system supports the signup and sign in feature. [error message with wrong credentials].
- User can send message to other user [p2p message] [ SEND command] [<SEND><USERNAME><MESSAGE>]
- Each user can join multiple chat rooms (groups) at a time.
- Each user can list all the groups.  [LIST Command] [show all group and number of participants ineach group]
- Each user can join a group [JOIN command]. If the group does not exist then the first create it thenjoins it.
- Each user can create a group [CREATE command].
- If one user sends a message to a group it should be sent to all members of that group.
- The message is encrypted using Tripple DES (3DES) and the key will be Diffie–Hellman key typeexchanged between clients.
- Each group has one key (random nonce).
- Message can be any type, for example, text, images, video, and audio.



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



