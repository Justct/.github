## Just Chat 

<p align="right"> <img src="https://komarev.com/ghpvc/?username=darkmash-org&label=Project%20views&color=0e75b6&style=flat" alt="darkmash-org" /> </p>


A simple open source site hosted via github pages  <br>
And via random people contributing a chat room .<br>
Here you can talk to random people with common <br>
Interests, Ideologies, and so on.<br>
<hr>
You can log into any chat room which you will be interested from <br>
The site "https://justct.github.io/". Here you can explore and   <br>
Filture out rooms which you would be interested in and so on. <br>
<br>
The chat site have a basic Interface. <br>
It only provides you a temp username, <br>
Note :  Only one person with a      <br>
username can join a specific room.    <br>
<br>
And only 3 people can join from the  <br>
same IP at a time, on to the same  <br>
chat room.
<br>
<br>
<i>Official API Url</i> : `https://backendjustchat.darkmash.repl.co`

#### How to -  Host a chatroom ?
Requirements  - python3 , pip3/pip , git

**Note : If hosting on replit use something like uptimebot to keep it alive**
```sh
git clone https://github.com/Justct/Chatroom.git
```
```sh
cd Chatroom
```

If on **replit** use this instead :

```sh
git clone https://github.com/Justct/Chatroom-replit.git && sed -i 's|entrypoint = "main.py"|entrypoint = "Chatroom-replit/main.py"|' .replit
```
```sh
cd Chatroom-replit 
```

```sh
pip install -r requirements.txt
```

Use python/python3 to run the Chatroom, If on replit use the 'run' button!
```sh
python main.py
```

After doing this register your Room here : https://justct.github.io/creation.html

#### How to -  Use the offical API ?

API url : `https://backendjustchat.darkmash.repl.co`<br>

Uses `GET` :

**/find/\<room name\>**
- Get API Url of the room in return

**/get/<int:page>/<int:results_per_page>** 
- Get the rooms
- Returns : JSON List of rooms + details
- Example return : 
  \[
  {"name":"chat room 1", "description": ".....", "api_url": "https://......"}
  \]
  

**/search/<string:search_query>** 
- Search for rooms- 
- Returns : JSON List of rooms + details
- Example return : 
  \[
  {"name":"chat room 1", "description": ".....", "api_url": "https://......"}
  \]



Uses `POST` :

**/new** 
- Creates A new chat room
- Headers should contain valid `name` and `api_url` and `description`
- Returns -  
   - "n" if the api url not working
   - "x" if a room with same name exists
   - "s" if it was a success

<hr>

##### Note
- Right now, if you wanna take your room down you have to join our discord and request for removal 

##### Discord server
Join our discord server to talk about the <br>
project and for giving us suggestions. <br>
<a href="https://discord.gg/SC54bSgnyQ">Join Server</a>

Project owned and managed by <a href= "https://darkmash-org.github.io/" >darkmash-org</a>
