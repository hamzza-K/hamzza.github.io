

# DashBoard Enhancements

- **logging each message sent by an agent**


![logging messages](/images/loggingmessages.png)

Agents monitoring the routed chats sometimes pitch in statements to engange the visitor till the actual owner of the chat picks it up and once in a while, they are constrained to end the chat. The responses sent in the chat cannot be distinguished whether they were sent by the actual owner or the agent monitoring chats which ensue complications in chat quality and handling reports (one of my chats reviewed were of such case; I did not handle the whole chat and it affected the overall rating). It would be better to add a functionality which can identify the reponses.


- **Adding more features**


Currently there are only 


# Security and Privacy Issues

- **Account getting locked-out**

![Dashboard Form](/images/loginform.png)

Inserting wrong password thrice can get your account locked, which may take several minutes or hours in some cases to retrieve it. Now, imagine a scenario where at a particular time, all agents get locked out of their accounts (using just a simple python script); **_Catastrophic!_**, the amount of damage it would cause us would be unfathomable.
From the inception of our company, we have acquired over 10000+ clients by sheer hardwork and being persistence which is in itself is commendable but as we thrive and climb up the ropes the more we get in the radar of other competitors. Knowing man, one can do everything in their might to exploit and bring the other down.

![Insecure Warning](/images/warning.png)

Our web applications e.g web3 & web2 run on insecure connections which can easily be prone to MiTM (man in the middle attack) to hijack any data we send between the server and vice-versa. 
According to the statistics, 43% of cyber attacks target small business. [64% of companies have experienced web-based attacks](https://www.fundera.com/resources/small-business-cyber-security-statistics). 62% experienced phishing & social engineering attack. 59% of companies experienced malicious code and botnets and 51% experienced denial of service attacks. Thus, it should be our priority to secure these sites.

- **Visitor's contact details**

Apparently, there is an encrypting algorithm (which sometimes glitches and encrypts the zip/postal code) used which covers visitor's phone number and email but there are a few ways from which we can easily retrieve visitor's data.
1. Using Export option in history feature
![export](/images/exportdata.PNG)

Visitor's data e.g name, email and phone number is stored inside an excel sheet. By clicking on the cell, you can easily see the phone number.

![decrypted](/images/decrypteddata.PNG)

2. Translate Feature
[translate](/images/translate.png)

Rarely, clicking the feature translates an English chat to English which repeats every statement said by the visitor and agent except the contact detail do not get encrypted and can be shown. (I used the word "rarely" since in most cases I've seen, translate feature translates English chats to English when visitor provides with a wrong/correct zip/postal code or scribbles untangible words)


