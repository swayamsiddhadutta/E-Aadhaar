# E-Aadhaar
Identity based on blockchain implementing Aadhaar for citizens.<br>

Get along with <a href="https://docs.google.com/document/d/1DBmVrAgcvEfp89loYYR0B-SPobRZlqIwLHH7A9KZwh0/edit?usp=sharing"> Code Walkthrough </a> to get started.

<strong> This is codebase for pre final year project.Do not use without reference. </strong>

Frameworks used:<br>
truffle<br>
mocha<br>
chai<br><br>

In-memory blockchain used:<br>
Ganache<br>

Solidity files:<br>
aadhaar.sol -- Smart contract --> Contains structures that store the user data and functions that help access them.
<br>
Javascript Files:<br>
aadhaar.js --> referenced by login.html,signup.html<br>
admin.js --> referenced by admin.html<br>
aadhaarInit.js --> used to compile and deploy the smart contract(aadhaar.sol) on the ethereum test net.<br>

E-Aadhaar is a (proposed)decentralized form of the current Aadhaar system.The UIDAI(Unique Identification Authority of India)<br>
has been maintaining Aadhaar data of Indian citizens for more than 7 years now and it has shown some major loopholes in it's system.<br>
Most of these loopholes can be credited to the centralized architecture of the web where in we follow a client-server based architecture<br>
with large number of clients(Aadhaar holders) and minimal number of servers(clustered in a centralized location).Almost all the companies<br>
today follow this architecture where these compaies maintain huge clusters of servers where user requests are handled.<br>
<br>
For the Aadhaar database maintained by UIDAI, scaling is a big factor.The UIDAI has a huge responsibility of securing the information of more<br> than 1 billion citizens.The recent attacks on the Aadhaar database system have led us to believe that maintaining biometric information in a<br> central database seems to be very much a matter of concern.<br><br>

 
Below are some of the links to such cases :<br>
<a href = "https://www.zdnet.com/article/another-data-leak-hits-india-aadhaar-biometric-database">Another data leak hits Aadhaar biometric database</a>
<a href = "https://www.medianama.com/2018/05/223-aadhaar-leaks-list/">Aadhaar leaks list</a>
 <br>
E-Aadhaar aims to remove the problems caused by a centralized architecture by using the ethereum blockchain as the single source of truth<br>
which is maintained not by an organization but a community.This community consists of the users of the E-Aadhaar.The data of users is kept <br>safe with the users through a decentralized architecture where the Aadhaar data is stored by a large number of nodes but are verified <br>only by some selected administrators.<br><br>

The ethereum blockchain uses PoW(Proof of Work) to get things on the blockchain.But such a consensus mechanism cannot be used here because
<br>the government can't give control of such sensitive data to mining pools.This data should be pushed into blocks by some selected officials <br>but the proof of verification is held by each node and thus,each node would be able to verify the correctness of the work done by officials.
<br><br>

Basically this is a proposed idea and not at any stage of production and therefore the programs here are deployed on a test network and not on <br>the main ethereum network.We use a language called solidity to write <a href="https://blockgeeks.com/guides/smart-contracts/">smart <br>contracts</a> which form the backend of our dApp(Decentralized application).   
<br><br>
