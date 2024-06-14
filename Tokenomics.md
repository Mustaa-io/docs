# Tokenomics
The tokenomics of this project has been whiteboarded roughly to assess how yacht sharing would work, meeting the demands of owners, renters and contributers. Where "yachts", "yachting" and more are used please replace with whatever other asset you can think of that could be shared.  

## Autonomous child asset
### Overview
Our yacht sharing platform utilizes a dual-token system to facilitate fractional ownership, rental, and governance. The tokenomics are designed to ensure a balanced ecosystem that incentivizes participation, aligns interests, and promotes the platform's growth.

<img width="990" alt="Screenshot 2024-06-14 at 07 51 04" src="https://github.com/Mustaa-io/docs/assets/152909876/052348f9-1a10-49b9-aa1b-6c67a4a0410d">
Figure 1. This is overview of the Yacht "DAO".

### NFT - Fractional Ownership
LSP8 NFTs represent fractional ownership of yachts on our platform. Each yacht is tokenized into a fixed number of NFTs, with each NFT representing a specific fraction of the yacht's ownership. NFT holders are entitled to a portion of the yacht's usage time and rental income, proportional to their ownership stake. The LSP8 standard is used to create these unique ownership NFTs, ensuring they are easily identifiable and distinguishable.

Specific for yachting, the boat will have to be out of the water every year. This means that out of 365 days, or 52 weeks only 48 weeks can be used. This coincides nicely with 4 NFT owners, each having 12 weeks of time.

<img width="1264" alt="Screenshot 2024-06-14 at 07 51 24" src="https://github.com/Mustaa-io/docs/assets/152909876/c40e6d6a-5212-46e6-ba47-766f0352ff81">
Figure 2. How an owner can sell their "time token" on the free market.

### $SAIL Token - Rental and Redistribution
The $SAIL token is our time utility token, used for booking days on the yacht. NFT holders receive $SAIL tokens based on their fractional ownership, which they can use to book time for their own usage or sell to charterers. Charterers can purchase $SAIL tokens from owners (see Figure 2) to rent yachts for specific time periods. The LSP7 (Digital Asset) standard is used to create the $SAIL token, enabling efficient transfers and integrating with the LUKSO ecosystem.

When the "time token" is transferred to the yacht's LSP9 vault it is stored there until a specific date (decided by owners). The redistribution of "time token" occurs automatically through a smart contract. The "time token" is either all used or not. If the "time token" is not used, then maybe the simplest solution is a force claim the tokens to the yacht's vault and then redistribute evenly. However, say a renter has bought these tokens at fair market price with a few weeks left to use and misses this specific date, this would mean they do not benefit from the purchase. Therefore, the tokens value significantly drops the closer it is to a redistribution date. We would have to solve this.

## Parent DAO
<img width="1265" alt="Screenshot 2024-06-14 at 07 51 46" src="https://github.com/Mustaa-io/docs/assets/152909876/cb22766f-409c-4f0c-8130-82b6b71310ec">
Figure 3. How a parent DAO can govern and help child autonomous assets.

The parent DAO acts as the overarching entity that manages the yacht sharing ecosystem. It oversees multiple yacht UPs, each representing a specific yacht. The parent DAO is responsible for financing the purchase of these assets, maybe through the underwriting from a bank. It should assist in helping acquire new yachts and expand the platform's fleet. It also facilitates the onboarding of service providers, such as insurance companies and maintenance crews, to ensure the yachts are well-maintained and protected.
The parent DAO utilizes the LSP9 (Vault) standard to securely hold and manage funds for the ecosystem. This includes charter income, payments to service providers, and funds for yacht acquisition. The use of a vault ensures transparency, security, and efficient management of the platform's financial resources.

