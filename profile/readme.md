## Just Chat 

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
<br>
<i>Official API Url</i> : `https://backendjustchat.darkmash.repl.co`

#### How to -  Host a chatroom ?
Requirements  - python3 , pip3/pip , git, ngrok account (default option is use ngrok)

**Note : Set up ngrok + configure it first!** https://ngrok.com/  

```sh
git clone https://github.com/Justct/Chatroom.git
```

```sh
cd Chatroom
```

```sh
pip install -r requirements
```

Use python/python3 to run the Chatroom
```sh
python main.py
```

#### How to -  Use the offical API ?

API url : `https://backendjustchat.darkmash.repl.co`<br>

Uses `GET` :


***/get/<int:page>/<int:results_per_page>** 
- Get the rooms
- Returns : JSON List of rooms + details
- Example return : 
  \[
  {"name":"chat room 1", "description": ".....", "api_url": "https://......"}
  \]
  

***/search/<string:search_query>** 
- Search for rooms- 
- Returns : JSON List of rooms + details
- Example return : 
  \[
  {"name":"chat room 1", "description": ".....", "api_url": "https://......"}
  \]



Uses `POST` :

***/new** 
- Creates A new chat room
- Headers should contain valid `name` and `api_url` and `description`
- Returns -  
   - "n" if the api url not working
   - "x" if a room with same name exists
   - "s" if it was a success

<hr>

##### Discord server
Join our discord server to talk about the <br>
project and for giving us suggestions. <br>
<a href="https://discord.gg/SC54bSgnyQ">Join Server</a>

Project owned and managed by <a href= "https://darkmash-org.github.io/" >darkmash-org</a>
