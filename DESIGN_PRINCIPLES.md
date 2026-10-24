# Design Principles

Monocle Network is built on Monero, a decentralized, private, open financial network where participants transact directly with each other. This gives everyone equal and direct access to economic opportunity without fearing seizure or needing intermediaries. These are the key principles to follow when designing for Monocle Network.

These principles come partly from the technology itself and partly from the network's values. Although every touch-point is different, work on the application, markets site, website, and wiki should strive to follow these principles. Diverging from them should only be done with very good reason.

## Privacy

### Minimize collection of personal information, and maximize financial privacy

Monero provides strong transaction privacy at the protocol level, and Monocle Network extends that promise: peer wallets, trades, and activity are private by design and are never published. Design should protect this at every step.

A trading network does not need to know who its peers are. Strive to collect as little personal information as possible. When something is absolutely required, collect only the bare minimum, and consider whether it can be discarded when no longer necessary. If personal information is ever involved, be transparent about why it exists and how it will be used.

**Do**
- Design so that no personal information is ever required
- Assume everything a peer enters could become sensitive
- Route expectations around Tor: privacy is the default, not an option
- Warn peers clearly before they share anything identifying (for example, payment account details shown to a counterparty)

**Don't**
- Collect and store personal information not required for the functionality of the product
- Design flows that encourage peers to reveal more than the trade requires
- Treat privacy as a setting peers must discover and enable

## Self-custody

### Let peers control their private keys, with no risk of seizure or freezing of funds

The existing mental model of digital services is usernames and passwords held by a company with custody of funds and data. With every peer having direct access to the Monero network, there is no need to design products that require people to delegate control of their funds to middlemen. While it comes with greater responsibility, self-custody enables the open financial system of peer-to-peer exchange.

**Do**
- Let peers control their Monero and private keys directly
- Create an easy path to self-custody for newcomers

**Don't**
- Custody funds for peers
- Build flows where a peer's funds can be seized or frozen

## Security

### Provide appropriate and progressive security for all types of peers

Self-custody leaves the peer responsible for the security of their own wallet. They can only do a good job of that with appropriate tools and awareness of best practices.

Security is especially important when on-boarding people who are new to Monero. New peers are likely to start by storing small amounts, and may become comfortable holding more over time. Design should let a peer's security practices grow as their usage does: the wallet seed, the wallet password, and backups each deserve clear, well-timed guidance rather than a wall of warnings on day one.

Education and awareness are a big part of security. It is unrealistic to expect a beginner to absorb everything an experienced peer knows, so consider how to continuously educate in context.

Security is also a feeling. A polished, easy-to-use product that transparently communicates how it works helps peers feel secure.

**Do**
- Take safeguarding of peers' funds seriously
- Strive for no loss of funds, whether by negligence or theft
- Provide suitable backup guidance for newcomers
- Build with bad actors in mind
- Minimize risk of self-inflicted loss from peer negligence
- Continuously educate peers on best practice and risks

**Don't**
- Expect beginners to implement best practice backup strategies unprompted
- Underestimate the added *feeling* of security that comes from well-polished products

## Inclusion

### Build borderless products without location, language, or social barriers

There are no background checks, credit checks, or gatekeepers on Monocle Network. 

The network it should be prepared for many peers, including people unfamiliar with Monero. This means using plain and familiar language, explaining things in the context where they are needed, and not overwhelming people with technical detail.

**Do**
- Design products usable by the widest range of people possible
- Use plain language that people new to Monero can understand regardless of prior knowledge
- Educate in place, when people are presented with a new concept
- Treat peers of assistive technologies as first-class citizens

**Don't**
- Exclude people by building features that only work in certain countries
- Add technical detail that is not required knowledge, or unexplained technical terms
- Put all education up front and expect people to read and remember it

## Transparency

### Be open and transparent with how the product works, and open-source everything possible

A private, decentralized financial system puts the burden on peers to choose products they trust. Monocle Network makes this easier by openly sharing how it works, publishing wallet addresses and view keys, and open-sourcing its code so anyone can verify claims. Design should carry this spirit: clear, honest interfaces that show what the network does, what fees apply, and what happens at each step of a trade.

Be transparent with peers about risk too: trades settle between people, payment methods can fail or be reversed, and the Peer Security Reserve covers verified exploits.

**Do**
- Be open and transparent about how the product works
- Show fees clearly, before a peer commits to anything
- Let people verify claims by open-sourcing work when possible
- Explain what risks the peer is taking on, and how best to mitigate them

**Don't**
- Make claims that are not explained or verifiable
- Bury costs or risks behind vague language

## Decentralization

### Design products that keep the network peer-to-peer

Unlike traditional finance, Monocle Network does not require anyone to seek permission. There is no central point of control. Every peer running the application is a node on the network.

Design should reinforce this: peers trade directly with each other, infrastructure is provided by contributors rather than a central operator, and the network's strength comes from its peers.

**Do**
- Design flows that make the peer-to-peer nature of trades visible and understandable
- Encourage peers who run their own infrastructure where relevant
- Offer peers choice in what they connect to

**Don't**
- Introduce a single point of failure between peers and the network
- Build products that stop working if the project shuts down

---

*Adapted from the Bitcoin Design Guide design principles, [CC BY 4.0](https://bitcoin.design/).*
