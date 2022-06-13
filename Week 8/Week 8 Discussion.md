## WEEK 8 DISCUSSION

`You are opening an online store in a cloud environment.  What type of Cloud service(s) do you leverage to open your store? What are the security responsibilities of your cloud service provider?  What are your security responsibilities?  What are three security controls you might use to protect customers' credit card information? Assume that the information will need to be stored.`

If I was going to open a online store I would use a PaaS model since it provides shared security between the customer and the provider. The overall cost of a PaaS modeled system is relatively low and it enables little management over the hardware required to run the store. 

Overall it is simplest and easier models to setup and continue to use as long as the provider is good on there end with managing there servers, network, switches, security, etc. This is one of the drawbacks of the model because for some people not having direct control of your supporting servers, and network is a big problem. 

But if you pick a good provider that can maintain the standard that you want to employee then there is very little work for you, the customer. For example when constructing my online store with the PaaS model I would only be in charge of the application run on the cloud servers and the data stored on them such as user information, personal information, transactional information, etc. All transactional information should be encrypted from time of submission to limit any security problems for the users.

Even though the cloud environment is through one provider necessary systems should be appropriately isolated from each other using segregate servers. For example the transactional database should be separated from the web server and only open to authorized users and correct server to server protocols. Access controls and an access log could also help in aiding this security by showing who is accessing the encrypted data and dependant systems. 

Depending on the stores implementation user authentication methods might be necessary but since this is just a small web store those should only be required for system admins. 

