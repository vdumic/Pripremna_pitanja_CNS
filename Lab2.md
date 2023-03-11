# Lab Title: Man-in-the-middle attacks (ARP spoofing)

## Challenge Answers

- **Challenge 1:** [Insert answer here, i.e., a Chuck Norris fact]
- **Challenge 2:** [Insert answer here, i.e., a `password` to unlock the next lab]

## Other Relevant Information

[Insert here, if applicable]

## Lab Prep Questions and Answers

1. What is the Address Resolution Protocol (ARP), and what is its role in a network?

   - The Address Resolution Protocol (ARP) is a communication (TCP/IP) protocol which is used to discover physical address, such as MAC address, from a given IP address.

2. What is a Man-in-the-Middle (MitM) attack, and how does ARP spoofing enable it?

   - Man-in-the-Middle (MitM) attack is a general term for when an attacker positions himself between two entities in comunication. ARP spoofing enables it in a way that attacker finds out the MAC address of the entity in the communication.

3. How does an attacker use ARP spoofing to intercept network traffic?

   - An attacker uses ARP sppofing to intercept network traffic in a way that he presents himself as an entity whose MAC address he found out, so the whole communication is redirected over an attacker and he can supervise it.

4. How is the _cookie_ used to derive the encryption/decryption key?

   - The encryption/decription key is dervied from the secret value which is called the _cookie_. From the _cookie_ we find out the key and decript the challenge.

5. What REST API request do you need to send to the crypto oracle to get the secret \_cookie:?

   - GET /arp/cookie

6. How do you obtain the authentication token?

   - The authentication token is obtained by requesting it from the _crypto oracle_ server. We also have to authenticate by sending username and password.

7. How do you use the authentication token to obtain the _cookie_?

   - The authentication token is used when sending a REST API request in whose reply we get the _cookie_, because without the _cookie_ sending a request wouldn't be successfull.

8. What encryption mode is used to encrypt the challenge in this lab?

   - CBC encryption mode with AES cipher (AES-CBC).

9. What tool can you use to capture network traffic on a local network interface?

   - tcpdump tool
