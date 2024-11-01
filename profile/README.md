# nethercode

Our goal is to empower customers with greater control over their energy data, giving them tools to monitor usage at a more detailed level than ever before. By developing a system of IoT devices and nodes that connect to the blockchain, we can offer consumers a transparent, decentralized platform to view their energy consumption patterns. This allows them to track exactly where and when energy is used, make smarter choices to reduce costs, and compare their usage with similar households on competing providers. With this granular insight and secure data access, customers can choose the best provider for their needs and potentially negotiate better deals, fostering a more consumer-driven and competitive energy market.

## Table Of Content

1. [Background](#background)
1. [Being Smart](#being-smart)
1. [Keeping Users Safe](#keeping-users-safe)
1. [Pumping Gas](#pumping-gas)
1. [Considering Cairo Contracts](#considering-cairo-contracts)
1. [Resources](#resources)

## Background

The rising cost of living is putting real pressure on people’s wallets, affecting everything from groceries and rent to commuting and utility bills. While there are budgeting tools out there, many people still don’t have effective ways to track and manage their spending day-to-day, especially when it comes to recurring household expenses like energy and water. Often, bills for these essentials arrive at the end of the month with little to no breakdown of how the charges were calculated, leaving people in the dark about what they’re actually paying for. This lack of transparency tends to put the power in the hands of the utility companies, rather than the consumers.

Even though there are plenty of providers to choose from, the hassle of switching — and the uncertainty about whether it will actually save money — keeps many people stuck with the same supplier. Without clear data on how much energy or water they’re using and what it costs, it’s hard to know if switching would make any real difference.

But what if control became decentralized and shifted directly to the consumer? With a detailed, transparent breakdown of their energy and water usage, people could see exactly where their money is going. This kind of decentralized data access would enable consumers to negotiate better deals with providers or make smarter choices about switching, tailored to their specific needs. By decentralizing access to utility data, we empower consumers with the insight they need to foster a more competitive market, potentially leading to fairer pricing and more control over household expenses.

## Being Smart

Smart meters in the UK are part of the solution to improve energy transparency by automatically tracking electricity and gas usage in real time. Once installed, these meters connect to a centralized network, the [Data Communications Company (DCC)](https://www.smartdcc.co.uk/about-dcc/who-we-are/), which securely collects data from millions of households and relays it to energy providers. This setup removes the need for manual readings, providing consumers with regular updates on their energy consumption through an in-home display (IHD). However, because the system is centralized, consumers have limited control over how this data is used in interactions with providers.

The data transmission works through a network of sensors within the smart meter, which continually monitor energy usage. This data is encrypted and securely sent via radio waves to a local communications hub in the home, which then transmits it over the DCC network. This central network ensures data reaches the energy provider while keeping it private, yet the reliance on centralized control limits flexibility for consumers to manage or share their data independently.

## Being Smarter

Currently, energy data from smart meters is securely transmitted to a central network (like the UK's Data Communications Company, DCC), which relays information to energy providers. However, centralization means that customers have limited access to their data and rely on providers to interpret it for them, potentially creating a power imbalance. Integrating blockchain technology could enhance this by decentralizing data access, allowing customers to control and share their data on a secure, tamper-proof network.

## Keeping Users Safe

Storing sensitive data using a hybrid approach is essential for protecting user privacy and ensuring compliance with regulations. This will include:

1. **Hashing Credentials**: Only the hashes of user credentials are stored, transforming identifiable information into a fixed-length string that is difficult to reverse.
1. **Off-Chain Storage**: Sensitive personal identifiable information (PII) is kept off the blockchain in secure environments, ensuring that the blockchain does not contain any directly identifying data.
1. **Anonymized Data**: Usage metrics and analytics are anonymized or aggregated before storage, preventing identification based on energy consumption patterns.
1. **Access Control and Permissions**: Tamper-proof hardware enforces strict access controls, allowing only authorized parties to access sensitive data.
1. **Decentralized Identifiers (DIDs)**: Users interact with the system using unique identifiers that do not reveal their personal identity.

By implementing these measures, the hybrid approach effectively safeguards user privacy while facilitating secure data verification and sharing.

## Pumping Gas

Collecting continuous sensor data is essential for monitoring energy use and improving how we consume energy in real time. Using a Layer 2 solution greatly helps this process by allowing more data to be processed quickly and at lower costs. Layer 2 solutions handle transactions off the main Ethereum blockchain, which means data can be sent and received faster without slowing down the network. This allows for a large amount of sensor data to be recorded and analyzed quickly, giving users immediate insights into their energy usage. Lower transaction fees make it more affordable to manage this ongoing data flow, enabling users to easily track their consumption and make informed decisions. Overall, this setup helps users improve their energy efficiency while ensuring that their data is securely verified on the blockchain.

<!-- Zero-knowledge proofs (ZKPs) are used in ZK rollups to process large numbers of transactions on blockchains -->

## Considering Cairo Contracts

Our system leverages the power of StarkNet and Cairo, enabling secure, decentralized tracking of energy data through IoT devices, like smart meters, installed in homes and businesses. By utilizing zero-knowledge proofs (ZKPs), our platform allows users to verify their energy usage publicly without revealing personal details. This means they can trust that their data is accurate and untampered without sacrificing their privacy. We empower users to view exactly where their energy costs are coming from and make data-driven choices, like negotiating better rates or even switching providers—all while keeping sensitive information secure.

The backbone of our solution is StarkNet’s Layer 2 technology, which processes high volumes of sensor data quickly and affordably by bundling multiple transactions for efficient verification. This technology enables us to collect continuous data from smart sensors at a fraction of the typical cost, passing those savings directly to our users. In an era where high gas fees make frequent data updates costly, our solution provides the scalability and cost-efficiency that real-world applications need.

## Resources

1. [nethermind](https://www.nethermind.io/)
1. [cairo-lang](https://www.cairo-lang.org/)
1. [dock: verifiable credentials](https://www.dock.io/post/verifiable-credentials)
1. [how cloudflare auto mitigated world record 3.8tbps ddos attack](https://blog.cloudflare.com/how-cloudflare-auto-mitigated-world-record-3-8-tbps-ddos-attack/)
