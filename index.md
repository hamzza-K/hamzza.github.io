






# DashBoard Enhancements
> I made this report based solely on my own observations and taking feedback from other agents that I know.

### **logging each message sent by an agent**


![logging messages](/images/loggingmessages.png)

Agents monitoring the routed chats sometimes pitch in statements to engange the visitor till the actual owner of the chat picks it up and once in a while, they are constrained to end the chat. The responses sent in the chat cannot be _distinguished_ whether they were sent by the actual owner or the agent monitoring chats which ensue complications in _chat quality_ and _handling reports_ (one of my chats reviewed were of such case; I did not handle the whole chat and it affected the overall rating). It would be better to add a functionality which can _identify_ the reponses.


### **Adding more features**

###### Different Sound for every new Chat assigned to us

![show](/images/showvisitorresponseinrealtime.png)

Currently, there is only one option (Enable/Disable sound) for every chat that appears i.e routing and new. Consider a common scenario where some agents gets disconnected due to internet issues. Their chats would start routing and at the same time some new chats get assigned to you but you are currently handling 10 chats (after 6/7 chats, you need to scroll to the right to see the remaining chats; depending on the screen width). There is a probability that those chats were easy sales but due to the high response time, they leave the chat. Also, constantly hearing the same sound is nerve-wrecking (when you are already tired).

> Also, why do we have an option to "turn on visitor's response in real time"? this option is equivalent to "You have two legs, but you can walk with one"

### **Tweaking some of the features to Improve efficiency**

###### Fixing the Address/location tree in chats

![address](/images/addresslocationnull.PNG)

Scenario: Sometimes a visitor comes back to a new chat right after finishing/ending the previous one saying, "call disconnected, please connect me again". It is optimal to connect them right away instead of asking about their location. But when it we send the lead, the system makes it mandatory to insert in the location even though the visitor did not provide it and most importantly, the option is not clicked. Forcefully, we have to insert some text to send the lead.

![keyfacts](/images/keys.PNG)

###### Refreshing a chat

![refreshing1](/images/refreshingachatp1.PNG)


We use refresh features to automatically add visitor's responses, email and phone number _when_ they are in the format i.e encrypted. But when they are not, we have to fill in the cells manually. Also, visitor's name gets removed everytime the chat is refreshed. 


![refreshing2](/images/refreshingachatp2.PNG)

### Removing Auto-responses

From what I've heard on the floor, handful of the agents are vary of auto-repsonses as they mess up their chats. I, from my experience, go against this feature (I had a chat where a 'must say' question was asked right in the beginning before getting assigned. Visitor ignored that must say and proceeded with the chat. At nigh end of the chat, I asked the same 'must ask' question to remove any confusion _But_ to my dismay, that 'must ask' had three auto-responses.. repeating every other statement that I pitched in the chat making the visitor aggravated in the end).

# Lumin the bot

In order to obtain maximum efficiency, I strongly believe that every task that can be automated, should be automated, and Lumin could greatly help us in that motive.

![lue](/images/luem.png)


# Security and Privacy Issues

### Account getting locked-out

![Dashboard Form](/images/loginform.png)

Inserting wrong password thrice can get your account locked, which may take several minutes or hours in some cases to retrieve it. Now, imagine a scenario where at a particular time, all agents get locked out of their accounts (using just a simple python script); **_Catastrophic!_**, the amount of damage it would cause us would be unfathomable.
From the inception of our company, we have acquired over 10000+ clients by sheer hardwork and being persistence which is in itself is commendable but as we thrive and climb up the ropes the more we get in the radar of other competitors. Knowing man, one can do everything in their might to exploit and bring the other down.

![Insecure Warning](/images/warning.png)

Our web applications e.g web3 & web2 run on insecure connections which can easily be prone to MiTM (man in the middle attack) to hijack any data we send between the server and vice-versa. 
According to the statistics, 43% of cyber attacks target small business. [64% of companies have experienced web-based attacks](https://www.fundera.com/resources/small-business-cyber-security-statistics). 62% experienced phishing & social engineering attack. 59% of companies experienced malicious code and botnets and 51% experienced denial of service attacks. Thus, it should be our priority to secure these sites.

### Visitor's contact details

Apparently, there is an encrypting algorithm (which sometimes glitches and encrypts the zip/postal code) used which covers visitor's phone number and email but there are a few ways from which we can easily retrieve visitor's data.
###### 1. Using Export option in history feature

![export](/images/exportdata.PNG)

Visitor's data e.g name, email and phone number is stored inside an excel sheet. By clicking on the cell, you can easily see the phone number.

![decrypted](/images/decrypteddata.PNG)

###### 2. Translate Feature

![translate](/images/translate.png)

Rarely, clicking the feature translates an English chat to English which repeats every statement said by the visitor and agent except that the contact details do not get encrypted and can be shown. (I used the word "rarely" since in most cases I've seen, translate feature translates English chats to English when visitor provides with a wrong/correct zip/postal code or scribbles untangible words)

###### 3. Intercepting our insecure web2 and web3 applications

![wireshark](/images/wireshark.png)

Tools like Burpsuite or wireshark can easily retrieve any packets containing sensitive data from web. Consequently, it is much easier to attack a deprecated unsecure HTTP server then a secure HTTPS server.

