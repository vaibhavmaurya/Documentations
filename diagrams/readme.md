# Table of Contents
- [Secure workflow using Self Sovereign Identity](#secure-workflow-using-self-sovereign-identity)
- [ML Model Discovery, Subscription and Consumption Platform](#ml-model-discovery-subscription-and-consumption-platform)
- [Service Market Place](#service-market-place)
- [User Subscription to Published Applications](#user-subscription-to-published-applications)
    - [Subscribed Application Resolution](#subscribed-application-resolution)


## Secure workflow using Self Sovereign Identity

There are two aspects, needs to be put here before making any statement about the idea.

### HTTPS/SSH/TLS Secure channel
We are pretty much familiar with the SSH/HTTPS/TLS protocol for secure communication over TCP. SSH communication is purely client server based communication where client and server both agrees with the symmetric key  and encrypt and decrypt the message. The meesage passes through the internet but in encrypted form.

Currently all known clients like browser or terminals are moving towards secure channel. Though as a user, I have no control over this communication, it is purely automated between client and server.

The symmetric key is valid between client and server. Usually HTTPS communication terminates at the server/client.

### User Identity and Authentication

Currently there are various methods two identify and authenticate a user. Let's take an example of a cancer hospital, which manages the cancer patients. The hospital has given an app, which patient uses to track their bookings and progress etc. This is a typical B to C app use case. Hospital has to maintain the user database, which would be identity provider. This user database contains user's information after pre-requisite verifications. Patient logins to the app and access it's progress. 
Here user data is centrally managed my hospital, which is prone to data leak. Patient's data like treatment, location etc can be leaked and so there would be to much effort to secure the central database and make it highly resilient to failure.

**Hospital**

- Is database safe for data leakage.
- Patient's trust on hospital that its data is safe and tamper proof
- Is database resilient and fault tolerant

How to recover the data if lost and make the data extremely resilient.

**Though the high resilientcy and security can be achieved using Cloud Providers Services. So let's check the alternative solutions and later compare the pros and cons**

**User**

- May loose the password.



### What if 

**User**

- Identity is maintained by patient only and patient does not shares it's data to hospital to maintain.
- Patient knows very well that hospital has no such its information which can be shared.

**Hospital**

- There are several copies of patient data which is encrypted and copied to multiple locations may be geographically or even in public places. Here the challenge is if data is copied to several location, is it possible to reconstruct the data in case of failure.
- There is no way to backtrack the user's identity from the transactional data stored with Hospital. See fromy the Hospital's angle, in the database there is a assumed user, though at user's angle user knows that its his/her data.


Now is there a way that patient/hospital creates an pseudo identity and agreed to communicate using this identity for communication after verification.
Though one can argue that there is always an pseudo identity like account number, cusotmer ID etc.

What if the identity can be used to create a secure channel like SSH but not like in a one single channel. Here the channel can be a workflow. 


Let's take an example patient has booked an appointment with the Doctor, What if a system faciliates a walkie talkie between patient and doctor over internet and the transactions are saved encrypted to any storage(can be public) but the key to decrypt resides with the stakeholders.

- How to protect from Data Leakage


## ML Model Discovery, Subscription and Consumption Platform





