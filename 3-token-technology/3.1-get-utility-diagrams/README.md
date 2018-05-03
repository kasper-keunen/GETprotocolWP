# 3.1 GET utility diagrams

Below are two high-level diagrams that illustrate how users and event organizers interact with the GET Protocol, and how GET facilitate these interactions. Figure 4 shows the GET utility of the most common protocol case: a consumer buying and using a ticket for an event. Table 6 lists the contracts displayed in the diagram. The bullet points describe the steps A-E that are taken by an end user who buys a smart ticket on the protocol. 

The diagram in Figure 5 below describes the secondary market mechanics happening on the GET Protocol. If an user with a ticket wants to sell their ticket, the smart ticket can be offered to the event-specific secondary market built into the protocol. In this event-specific secondary market, tickets are sold for their original selling price alongside the tickets of the event organizer \(also known as the primary ticketing market\).

| Contract | Description |
| --- | --- | --- | --- |
| 1 | Event Ticketing Contract \(ETC\) - This contract is owned by the event organizer. In addition to being the instantiator and
| 2 | Primary / Secondary Market Contract \(PSMC\) - This contract acts as a central matching market for both the tickets sold
| 3 | User Smart Ticket Contract \(USTC\) - This contract manages the GET users with valid tickets and is responsible for serving the QR code to users with these tickets right before the event starts. For providing this service the contract receives GET from those who use the contract. |

_Table 6: Functions and roles of the three contracts labelled in Figure 4 below._

![Figure 4](../../.gitbook/assets/image%20%2811%29.png)

_Figure 4: The process of consumer verification and the purchase of a smart ticket on the GET Protocol. Note

## Step A-E of Figure 4 explained.

* A: An unknown customer enters the protocol with the intention to buy a ticket. If the user’s phone \(or web browser\) is unknown to the protocol after signing in \(meaning the user never used his phone to buy
* B: In the account creation phase \(A\) the user has provided the protocol with a phone number. In
* C: At this point the user will be shown an interface in which he or she is able to pay for the ticket using
* D: After payment is completed, the API will send the required amount of GET tokens to the USTC
* E: At the event horizon \(the moment an event begins\) the PSMC contract activates all of the users’ smart

![Diagram 5](../../.gitbook/assets/image%20%2810%29.png)

_Figure 5: The mechanics of secondary ticketing market. Note that both the seller of the smart ticket as well
