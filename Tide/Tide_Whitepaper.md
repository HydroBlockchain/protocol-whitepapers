
# HYDRO TIDE: IDENTITY-LINKED PAYMENTS
## May 2019

# [TABLE OF CONTENTS]

  

[Abstract](#abstract)

  

[Background](#background)

[Mobile Payments](#mobile-payments)

[Point of Sale Payments](#point-of-sale-payments)

[History of P2P Payments](#history-of-p2p-payments)

[Remittance](#remittance)

[Problems with Traditional Payments](#problems-with-traditional-payments)

[Fraud and Chargebacks in Traditional Payments](#fraud-and-chargebacks-in-traditional-payments)

[Introducing Tide](#introducing-tide)

[Snowflake and ERC 1484](#snowflake-and-erc-1484)

[P2P Payments](#p2p-payments)

[Subscriptions](#subscriptions)

[Hydro Tide Subscription Smart Contract](#hydro-tide-subscription-smart-contract)

[Interest Payments](#interest-payments)

[Hydro Tide Interest Payments Smart Contract](#hydro-tide-interest-payments-smart-contract)

[Coupon Payments](#coupon-payments)

[Hydro Tide Coupon Smart Contract](#hydro-tide-coupon-smart-contract)

[Gift Cards](#gift-cards)

[Hydro Tide Gift Card Smart Contract](#hydro-tide-gift-card-smart-contract)

[Remittance Payments](#remittance-payments)

[Lottery and One-Time Payments](#lottery-and-one-time-payments)

[Invoicing AR and AP](#invoicing-ar-and-ap)

[HYDRO Tokens In Tide](#hydro-tokens-in-tide)

[Implications of Tide](#implications-of-tide)

[Consumer Applications](#consumer-applications)

[B2B Applications](#b2b-applications)

[Tide Partnerships](#tide-partnerships) 

[Native Mobile QR Codes and NFC](#native-mobile-qr-codes-and-nfc)

[Risks](#risks)

[Conclusion](#conclusion)

[Sources](#sources)

  

## Abstract

========

  

Hydro's mission is to provide blockchain solutions to businesses and blockchain projects, empowering a new decentralized global economy. The Hydro ecosystem consists of smart contracts and protocols that can be used by a variety of applications across fintech, logistics, healthcare, iOT and many other areas. Hydro enables companies to leverage the advantages of blockchain technology within their existing and future systems, reducing the need to hire blockchain developers.

  

A core component of any business ecosystem is the need for payments that are verified, linked, and recorded between users. The traditional banking and credit system has been unable to serve a large part of the world's population. Blockchain payment systems that have been introduced lack interoperability, both with other blockchains, and with existing and legacy payment systems. Very few applications have been able to successfully bridge the gap between underlying blockchain infrastructure and the real world.

  

In this paper, we propose smart contracts linked to the Hydro ERC-1484 identity standard, what we call "identity linked payments." These smart contracts will make it easier to create real-world decentralized applications to facilitate identity linked payment functionalities across point of sale, e-commerce, credit, and traditional payment systems.

  

Potential Hydro Tide Use Cases:

  

1.  P2P payments

  

2.  Global Remittance

  

3.  Subscriptions

  

4.  Interest and Dividends

  

5.  Coupons

  

6.  Lotteries

  

7.  Gift Cards

  

8.  Invoicing

  

As projects on Ethereum, such as Plasma, achieve faster transaction throughput, and native mobile wallets become prevalent, payments using blockchain technology will be intertwined with our everyday lives. Blockchain gives us a massive opportunity to bring payments to billions of unbanked people around the globe. Combining blockchain technology with a simple integration toolkit for developers, and products exhibiting great user experiences, Hydro Tide will power the Web 3.0 payments revolution.

  

## Background

==========

  

The idea of digital cash was first advanced by David Chaum in his 1983 paper "Blind Signatures for Untraceable Payments"[1].  In this paper, Chaum proposed a technique for storing digital cash and sending payments to other users, with a central bank cryptographically signing the secure transfer. In 1990, Chaum founded DigiCash, and with it, the ecash payments system. The ecash system was groundbreaking. For the first time, cryptographically secure, private, online P2P payments were possible. As groundbreaking as the ecash system was, it struggled with adoption, and as often happens with early technology, the company failed. Digicash filed for bankruptcy in 1998 [2].

  

As the Web 1.0 continued to grow, novel micropayment systems, such as those from Ecash and Millicent, tried and failed. It became clear that these early online payment services (which required in-depth knowledge of data transfer protocols) were complicated, lacking trust and interest from bank customers, prohibiting mainstream adoption. If the technology was to move beyond the capabilities of banks and other technologically-adept companies, and into the hands of the public, something had to change.

  

This change came with the advent of Web 2.0 in the late 1990s and early 2000s. This period witnessed the rise of internet giants such as Google, Amazon, eBay, and PayPal, and with these the rise of accessible, simplified, online payment systems; online payments had finally reached mainstream adoption.

  

The early days saw a battle for supremacy between auction site eBay and payments startup PayPal. The auction site had been identified by PayPal as an easy place to pick up a user base, and Paypal created such waves that eBay launched their own payment service in competition. However, PayPal had already made a lasting impact, not just via its payments system, but through groundbreaking innovations such as email payments and CAPTCHA security.

  

So big was the impact that in 2002, eBay purchased PayPal for $1.5 billion. The acquisition has since paid for itself many times over; in 2017, PayPal reported a revenue of over $13 billion, around 8.6x the initial cost to eBay. Alongside PayPal, companies such as Square, Venmo, and Braintree have captured a large chunk of the multi-billion dollar market and, in the case of Braintree and Venmo, have been acquired by PayPal in multi-million dollar deals [3].

  

More recently, we have seen online payment startup Stripe launch in direct competition to PayPal. The Stripe model was well-designed, simple to use, and provided APIs that allowed web developers to quickly add payment processing functionalities to websites and mobile apps. These are all areas that PayPal had struggled with in the past. Over the past year, Stripe has grown by adding simple customer migration tools, anti-fraud tools, incorporation tools, credit card issuance, and Stripe-enabled credit card terminals. According to Techcrunch, Stripe is now valued at $22.5 billion [4]!

  

The online payments market is one of the largest market sectors and shows no sign of stalling. With the increasing utility of trustless payment systems in combination with machine learning and open-source protocols, we are witnessing the advent of the Web 3.0. With it comes an opportunity for further growth via secure, identity-linked, online payments systems.

  

## Mobile Payments

---------------

  

Mobile payments have become one of the most convenient and accessible online payment methods, available across all demographics. This is not surprising, given that approximately 62.9% of the world's population now owns a mobile phone, with mobile phones usage predicted to surpass five billion in 2019[5].

  

By 2021, the use of  smartphones to make in-store payments is expected to generate close to $190 billion in transaction value in the United States alone. However, it is not only wealthy, developed nations leading the charge; the unbanked and underbanked represent significant growth areas, with micropayment solutions making a massive impact in developing countries.

  

This was first seen with the rise in popularity of the M-Pesa system in Africa. Since its first release in Kenya in 2007, M-Pesa has spread to over seven countries, and reportedly moves in excess of $36 billion USD per year. BitPesa has underscored the global demand for mobile payment options and mobile wallets. After first launching those products in Kenya in 2014, BitPesa has evolved to provide BTC payments and cross-border settlement to eight countries in Africa.

  

Reports indicate that the global mobile payments market reached $601.3 billion in 2016, and is forecast to reach $4.57 trillion USD by 2024[6]. We will examine blockchain's potential to power this ecosystem in this paper.

  

## Point of Sale Payments

----------------------

  

The first widely-recognized point of sale (POS) system was created in the 1870s by James Ritty, allowing users to press a key that represented and counted a specific amount of money. POS systems transformed greatly since the days of steamboats and railroads, and by the 20th century were a staple in nearly every reputable business.

  

By the 1970s, computer-based POS systems emerged and began to form the foundation for a retail-centric economy, allowing for efficient interaction, such as with barcode scanners. Touchscreen systems followed in 1986, and full graphical user interfaces in the 1990s. The Internet expanded POS functionality and POS systems became a software-as-a-service (SaaS) product. Cloud-based systems, NFC payments, and tokenization systems like Apple Pay have since emerged, demonstrating the continued demand to introduce greater efficiencies and utility.

  

POS systems have flourished greatly as technological advancement has kept stride with the demand for shopping. In 2018, over $6 trillion dollars in retail sales were reported, according to U.S. Census data. In the same manner that POS is transitioning to cloud-based systems, consumers have seen a boost of online shopping of over 300% in the past 20 years. In 2018, an estimated 1.8 billion people made an online purchase, and roughly 24% of the world population now has access to online POS systems [6.5].

  

## History of P2P Payments

------------

  

Peer-to-peer payments, typically referred to as "P2P" payments, are transactions  involving two people as the sole direct participants of the transaction. Although history points to P2P theory within legacy barter systems, electronic P2P payments and transactions were not prevalent before their mainstream introduction by PayPal in 1998. Paypal became a success within its first five years of operation, bringing in $1.5 billion dollars. Paypal's P2P payment engines significantly altered the way we exchange money, previously constrained by banks that forced users to wait for transfer approval and week-day settlement.

  

Not long afterward, the smartphone industry challenged the way we considered payments, and P2P payments became a mainstream concept. Companies like Square, Venmo, and Zelle surfaced, exemplifying the demand for more efficient systems, and P2P payment volume for PayPal alone reached $578 billion dollars in 2018 [7].

  

Most recently, with the creation and progression of cryptocurrency and blockchain technology, the P2P architecture of blockchain has proven itself as a solution to system redundancies and inefficiencies. Decentralized blockchain systems allow for the disintermediation of central hubs and controlling actors, making them one of the purest peer-to-peer payment solutions to date.

  

## Remittance

----------

  

Payments, funding, and money sent or received abroad are referred to as remittances. The concept and practice of remittance is an ancient concept, demonstrated by Spain and Italy in the 19th century, sending money overseas from maritime conquest. Around the dawn of World War II, remittances became a significant portion of national economies, with Spain reporting 21% of income in 1946 being sourced from remittance funding[8].

  

Technology has allowed remittances to increase significantly in the 21st century, with $529 billion dollars reported worldwide in 2012; countries such as India and China made up for roughly $130 billion that year alone. Remittance is often an indispensable option for countries requiring emergency aid, or that are restricted by slower economic development [9].

  

The significant increase of remittances has caused many to evaluate the global economic impact of international money transference. In 2018, $462 billion was sent to lower-income families. Remittances have had a significant effect on the Gross Domestic Product (GDP) of many countries, as seen in Mexico in 2015, where remittance income outpaced national oil sales [10]. Bill Gates, founder of Microsoft, has argued that a 50% reduction in fees could unlock $15 billion to underdeveloped countries worldwide [11].

  

## Problems with Traditional Payments

----------------------------------

  

There have been significant constraints on legacy payments and transactions throughout history, especially in the past century, where mounting laws and regulations further constrained free money exchange. Traditional legal tender (cash and coin), are limited by their physical nature, and do not protect against the inherent risk of theft. Checks and money orders are plagued with problems as well. They are not legal tender, suffer from wait times for cleared transfers, and carry potential penalties for insufficient funds.

  

Since the invention of credit and debit cards, there has been significant progress, but card-based payments have also given rise to an array of new challenges. Early credit and debit card systems provided easy access to account information such as card numbers, but the convenience of card systems relies on the trust of third parties (often unknown to the card holder).

  

This way of storing data has allowed hackers to target companies and credit card databases (as well as individual card holders) to obtain account information and balances at an ever-increasing rate. As theft increased, security measures like PIN codes and holograms surfaced, but PIN codes were easy to steal and holograms became obsolete as internet shopping became popular. EMV chips have also acted as a security measure for in-person card payments, but still have their setbacks, with a lack of support due to frustration from slower checkout times.

  

## Fraud and Chargebacks in Traditional Payments

---------------------------------------------

  

Fraudulent payments and transactions within traditional finance systems can be traced back as far as the systems themselves. Counterfeiting techniques were prevalent in 600 BC in Greece, where coins were tested by shaving the sides to determine whether the metal was solid, before being accepted in trade. Paper money has undergone many anti-counterfeiting revisions to combat sophisticated copying methods, resulting in heightened expenses to maintain currency value, as well as the need for the retirement and redistribution of aged tender [12].

  

Card-based and current contactless payment methods are especially susceptible to fraud. Credit and debit card fraud have been closely associated with ID theft as well, making breaches damaging to consumers. Cards can be manipulated, obtained without proper identification or assumed identity, and goods and services can be purchased on credit without the intent or ability to pay back the debt.

  

Card systems and bank accounts have also been susceptible to chargebacks, returned funds on charges undergoing dispute, or fraud resolution processes. The original intent of chargebacks was meant to benefit the consumer. However, this has been abused by consumers asking for chargebacks in an attempt to receive goods or services without charge. Chargebacks are also susceptible to payments falsely charged to accounts multiple times, to accounts with insufficient funds, or to payments without authorization, leading to considerable consequences to payment processes and heightened transaction fees for honest users.

  

# Introducing Tide

================

  

As mentioned in the beginning of this paper,  payments that can be verified with a sufficient level of certainty, linked, and recorded between users are central to every economic ecosystem.

  

Tide is a payment protocol that includes built-in identity and authentication. Built on the decentralized and public Ethereum blockchain, Tide allows users to complete one-click authorization of debit and credit POS transactions, as well as instantaneous P2P, P2B, and B2B payments. In addition, all of these payments are secured by Hydro's Raindrop and Snowflake protocols, providing an unprecedented level of security.

  

Although Hydro and the HYDRO token lie at the core of the Tide payment system, by incorporating other protocols and technologies, such as atomic swaps, Tide is essentially cryptocurrency-agnostic.

  

All of the Hydro smart contracts are open source and free for anyone to use and build on, from individual developers, to large enterprises. Below we discuss Tide functionalities and how developers can integrate Tide into their systems. Included as well are some examples built by the Project Hydro team.

  

## Snowflake and ERC 1484

--------------------

  

A core component of Snowflake was the creation, by the Project Hydro team, of a new digital identity standard: [ERC-1484](https://github.com/ethereum/EIPs/issues/1495). The creation of ERC-1484 ensures that various identity standards across the Ethereum blockchain can be connected. In summary, ERC-1484 is designed as "a protocol for aggregating digital identity information that's broadly interoperable with existing, proposed, and hypothetical future digital identity standards."[13]

  

It has become evident that traditional dApp interaction has one fundamental flaw: fragmentation. Interaction with dApps across devices requires either the transfer of private keys to new wallets, or the creation of entirely new and unassociated wallet addresses (and transfer of funds) on the new device. This process is inconvenient, costly, and prone to user error. It also exposes a user's tokens, and any data tied to that address, to phishing and malware attacks.

  

A key feature of Snowflake and ERC-1484 is the capability for users to claim multiple Ethereum addresses through cryptographic signatures, and tie all of these addresses to their core Snowflake. This results in the ability to interact with any dApp across devices, eliminating the issues described above. This is called [Resolver Management](https://hydro.gitbook.io/docs/snowflake/resolver-management).

  

"Procedurally, when linking a new address to their Snowflake, the owner address initiates a signed claim sign (EIN, addressToClaim, timestamp). Subsequently, the address to be claimed sends a transaction with the signed claim, addressToAdd, and approvingAddress. The initial claim is timestamped in order to prevent a malicious observer from recognizing which address an owner is trying to claim prior to the completion of the claim."[(14])

  

So, how does Tide fit into this? As an example, when using the Hydro dApp Store, Snowflake allows users to streamline the development process for dApp developers who are aiming to include payment features without wanting to create sophisticated payment infrastructure within their dApps. For the first time, users are able to manage withdrawals of Hydro balancess for all of their resolvers without creating separate wallet solutions for each individual dApp.

  

Details about the broader background of ERC-1484 and how it ties into Snowflake can be found in the [Snowflake whitepaper](https://github.com/hydrogen-dev/hydro-docs/blob/master/Snowflake/Snowflake_DRAFT.md).

  

## P2P Payments

------------

  

We have seen the impact that personal P2P payments apps, such as Venmo, have had on the world of online payments. These apps have become popular, as they create a quick and easy way of sending money to friends and family. However, we have not yet seen a user-friendly solution for P2P crypto payments - and that's where Tide will make a difference.

  

An example of how Tide can power the P2P Payment market can be seen in the P2P mobile payments app developed by Hydro. The app provides instant, gasless, identity-linked P2P crypto payments, that leverage ERC-1484 to streamline the onboarding process.

  

The ERC-1484 framework is used to provide each user with a Hydro ID. This simplifies Tide transactions, as users are able to send payments directly to a shortened and individual ID, rather than a long and complicated address. This simplicity creates a more user-friendly onboarding experience, especially for first-time cryptocurrency users, and is just one of the unique selling points of apps and dApps built on Tide.

  

## Subscriptions

-------------

  

A very compelling feature of Snowflake is that Snowflakes permit users to set allowances for different applications. This means that once a user has tied their identity to a resolver, a convenient structure for Hydro transfer between that user and the resolver is established; in particular, it streamlines billing systems.

  

### Hydro Tide Subscription Smart Contract

  

The Hydro Tide Subscription Smart Contract has been designed to allow businesses to bill a consumer or other business entity a recurring HYDRO subscription amount through a number of features:

  

- Billing Plans - allows users to subscribe to a billing plan. e.g. 1,000 HYDRO per month, 2,000 HYDRO per month, or 3,000 HYDRO per month, and the user can select from platform-generated options.

  

- Cancellation and Modification - users may cancel, modify, upgrade, or downgrade subscription plans within the smart contract.

  

- Prorated Billing - calculates the amount of HYDRO within a current billing cycle. e.g. if the user gets billed on the first of every month, this function would calculate the amount of HYDRO being used for X days / Y days of the month.

  

- Tiered Pricing - non-linear pricing. e.g. up to 20 users is 1,000 HYDRO, up to 100 users is 2,000 HYDRO, and up to 1,000 users is 3,000 HYDRO

  

- Quantities - subscribe multiple people within a group to a plan. For example, say you run a hosting company through which customers host sites at a cost of $9.99 per site per month. Most customers host a single site, while some host many. You could create plans for one site ($9.99), two sites ($19.98), and so forth, or subscribe customers to a quantity of the base $9.99 plan.

  

- Discounts - reduce invoices by a percentage or a flat amount for every invoice, just one invoice, or for a certain length of time. Can also apply to every subscription a customer has or only specific ones.

  

- Trial Periods - delays payments on active subscriptions using trial periods. e.g. payment remains in a user's Snowflake for 20 days, and if they do not cancel the subscription it gets released.

  

- Taxes - if you need to collect any type of tax on a subscription, such as VAT or sales tax, you can add a percentage in HYDRO that can be converted back into the base fiat currency.

  

- Billing Cycles - recurring billing cycles that end on any calendar year, either monthly, quarterly, or yearly. e.g. 1,000 HYDRO is withdrawn from the Snowflake balance on the 1st of every month until cancelled.

  

- Multiple Subscriptions - multiple subscriptions for a single customer by subscribing them to more than one plan or different variations of the same plan. e.g. a single Snowflake address can be subscribed to a 1,000 HYDRO per month plan and a 5,000 HYDRO per month plan.

  

- Usage Transformation - charge X HYDRO for every Y user. e.g. 1,000 HYDRO for every 10 users. In this example, users 1-10 all get charged only 1,000 HYDRO by the business.

  

- Authenticate: To finalize any subscription payment, the Hydro Raindrop 2FA must be performed.

  

## Interest Payments

-----------------

  

The market for interest-bearing notes and accounts is enormous, and the market for interest-paying debt products is even larger. However, one of the largest problems facing the lending market is default.

  

Nearly 40% of all U.S. borrowers are expected to default on their balances within 5 years in the student loan market alone, and between 2008 and 2013, nearly 500 banks failed in the U.S., costing the FDIC $73 Billion to compensate for losses [15].

  

Tide can solve these issues by holding interest from an issuer or borrower in escrow within Snowflake, allowing counterparties to eliminate fraud, prevent default, and validate all terms on-chain.

  

### Hydro Tide Interest Payments Smart Contract

  

Features of the Tide Interest Payments Smart Contract include the ability to:

  

- Create Interest Rates between 0-100%

  

- Set the Principal Amount that the interest is calculated on

  

- Define Snowflake IDs for both the payer and the payee

  

- Set the accrual date for the interest payments

  

- Set the payment schedule for the interest payments

  

- Set the end date, or term, of the payments

  

- Remove the set amount of HYDRO from the SnowflakeID wallet to an escrow contract according to the payment schedule intervals, to insure there will be no default

  

- Send Interest by distributing the interest in HYDRO from the escrow on the Payment Schedule date

  

- Send the principal amount on the contract from the Snowflake ID on the End Date

  

- Use the Hydro Raindrop smart contract to confirm receipt and payment of the interest from the payer to the payee

  

- Create a flag for a disputed interest payment

  

## Coupon Payments

---------------

  

The Tide coupon smart contract allows businesses to create coupons with unique characteristics for their services, and for a user to redeem these coupons.

  

Coupons provide a percent-off or amount-off discount for a particular set of customers and are an important part of e-commerce, POS transactions, invoicing, and orders. An on-chain approach to coupons creates uniqueness, and eliminates fraud and disputes within the marketplace.

  

### Hydro Tide Coupon Smart Contract

  

Features of the Tide coupon smart contract include:

  

- Simple Marketplace:

  

- One-to-many; seller-to-buyer

  

- Seller is contract owner (admin)

  

- Seller can list items with set properties:

  

- Name

  

- Description

  

- Price

  

- Uid

  

- Item type

  

- Purchase listed items at-price by sending a transaction that:

  

- Calls allow-and-call for the user on Snowflake

  

- Sets an allowance equal to the price

  

- Draws the corresponding allowance from the user

  

- Transfers ownership of the item to the buyer

  

## Gift Cards

----------

  

Expected to reach over $1 Trillion in value globally, the gift card market is one of the fastest-growing commerce market sectors. However, gift cards also have some of the highest fraud rates in e-commerce, with 9.510% of all fraud attempts in e-commerce occurring through downloadable gift cards [16].

  

With Hydro Tide, a business can create gift cards for their services, allowing a user to pay for things in the Hydro ecosystem by using pre-loaded and pre-defined amounts tied to their Snowflake address.

  

### Hydro Tide Gift Card Smart Contract

  

Features of the Tide gift card smart contract include:

  

- Creation of the gift card by the issuer, including total number of gift cards to be issued, unique codes on the cards, ID of Snowflake for business entity, amounts available for each card, & date of expiry

  

- Exchange an exact amount of Hydro for a predefined value on the gift card by the purchaser

  

- Storage of an electronic record of the gift card amount in a segregated part of the Hydro user's Snowflake (much like an escrow contract), to ensure that users can't use the gift card anywhere where it is not intended to be spent, and it cannot be exchanged for fiat or other cryptocurrency.

  

- Only the user is allowed to draw down to the exact amount of the gift card, with the gift card being 'burned' at a zero value.

  

- Users can authenticate the gift card ID and redeem at selected merchants tied to that Snowflake ID

  

- Redemption of a gift card can only occur after Hydro Raindrop authentication

  

- Swapping or transferring of gift cards under conditions specified by the issuer

  

## Remittance Payments

-------------------

  

Remittance payments can be streamlined using Hydro Tide and ERC-1484. Traditional services like Western Union, and even upstarts like Transferwise, charge exorbitant fees for remittance. This is because of the many middleean involved, each taking a slice of the pie as the money is moved in between parties. Blockchain gives us the ability to create a more decentralized remittance ecosystem.

  

Hydro Tide smart contracts can be built to allow developers to build remittance dApps that move HYDRO tokens in between Snowflake addresses of users in different countries, with swaps built-in for stablecoin (and potentially fiat) on-ramps and off-ramps. Thanks to ERC-1484 senders guarantee their payment arrives, business providers can guarantee funds are available, and receivers are able to use the received cryptocurrency immediately. As decentralized cryptocurrency markets become more mature, these remittance dApps can be provided with virtually no middleman fees to the end user.

  

## Lottery and One-Time Payments

-----------------------------

  

The Hydro Tide lottery smart contract has been designed so that Snowflake EINs can create unique lotteries, where rewards are in the form of HYDRO tokens.

  

The smart contract has been built as a Hydro Escrow contract, a Randomizer contract that uses an oracle for creating secure randomized numbers, with the main logic being controlled by an overarching Hydro Lottery contract.

  

To get over the security risks associated with creating fully-randomized numbers on the blockchain, the contract uses an external oracle, which charges a small amount of ETH everytime it generates a random number.

  

## Invoicing AR and AP

---------------------

  

The e-invoice market is expected to grow to over exponentially in the five years, and by validating, authenticating, and cutting down on transaction fees, blockchain technology has the potential to disrupt this market.

  

The Hydro Tide Invoicing smart contract has been built to serve this market, by allowing a business to invoice other businesses, or consumers, for a specific amount, on a specified date, and with a set amount of HYDRO.

  

## HYDRO Tokens In Tide

--------------------

  

The movement of HYDRO tokens as a payment solution is perhaps the most simple and most common use case in the Hydro ecosystem; however, there are many other applications of the  Hydro token within Tide, including:

  

1.  Subscription: When a user wants to pay for a subscription or recurring payment for something, they will use HYDRO tokens to pay the service providers, whether on a daily, weekly, monthly, annual, etc. basis

  

2.  Interest: HYDRO tokens can be held in escrow for interest payments, helping to prevent fraud

  

3.  Coupon: POS companies and businesses can use the coupon smart contract to give discounts on purchases using HYDRO in brick and mortar or e-commerce marketplaces

  

4.  Remittance: ability to send money to anyone around the world by using HYDRO

  

5.  Lottery: Smart contract for random number generator where the reward is paid out using HYDRO

  

6.  Invoicing: Companies can create invoices and charge payments in HYDRO on a certain date, and request a specific amount

  

7.  Gift Cards: Brick and Mortar and e-commerce stores can preload a certain amount of HYDRO and tie it to a user's Snowflake, which can be used to purchase physical or digital goods

  

The HYDRO token is the driving force behind Tide and is essential to all payments through the Hydro Ecosystem. By encouraging massive business adoption through easy to use toolkits, APIs, and Layer-4 platform creation, the Projet Hydro team can make HYDRO an accepted form of payment globally, especially in markets with large unbanked populations. This will lead to lower fees, faster economic growth, and higher standards of living for many lower income business owners. The Hydro token will always be at work in the background to ensure the system runs smoothly and securely.

  

# Implications of Tide

====================

  

The entire Hydro ethos is embodied in making blockchain solutions available to everyone, providing developers with easy-to-implement tools to build apps that use blockchain without customers even knowing it. Tide is no different, bringing blockchain payments to the next level. Tide is the central hub for HYDRO-powered crypto payments. Until now, online payment technologies have relied on disjointed services, from third-party authentication, to long and arduous KYC applications, with blockchain solutions facing the additional barrier of multiple, unlinked, wallets, all requiring their own individual gas costs.

  

The Hydro ecosystem, with the addition of Hydro Tide, allows for an all-in-one payment experience, from setting up accounts with Snowflake to completing all types of transactions. Furthermore, by using blockchain technologies such as Chainlink, Uniswap, and atomic swaps, hydro will power payments not only across ERC20 tokens, but also across chains and traditional payment services.

  

## Consumer Applications

---------------------

  

As mentioned in previous sections, the first Tide consumer applications have already been developed by Project Hydro, on top of public Hydro protocols.  Moving forward, it is envisaged that an increasing number of third-party developers and enterprises will use the Tide protocols to increase the security, flexibility, and interoperability of their consumer product lines. With the above advantages in mind, the consumer will not be the product, as often seen within data-driven systems that rely on user data as a revenue stream, but rather will benefit from increased efficiency, lower fees, greater security, and access to more robust, utility-oriented systems.

  

The advantage of Hydro Payments in consumer application is the ease of use for the user, who will not need to be proficient in blockchain to participate in the P2P payment revolution. Tide Payments streamline the payment process in the most efficient way possible for the user. This simplicity combined with effective security will provide a great bridge for consumer adoption.

  

## B2B Applications

----------------

  

More and more startups and enterprises are moving into the blockchain space, testing and leveraging blockchain technology to their advantage. The Hydro protocols provide a shortcut for these companies to integrate blockchain technology, without the need for blockchain developers. However, legacy businesses of all sizes could take advantage of this kind of adoption as it allows them to work smarter, faster, cheaper, and in a secure manner, while also offering the benefit of decentralization, so that one business in particular cannot take advantage of the other.

  

## Tide Partnerships

-----------------

  

With the Hydro ecosystem beginning to flourish, certain solutions can help our ecosystem grow and become completely autonomous. When looking at Ethereum and the scalability of its main chain, microtransactions are not always going to be the best fit. Scalability solutions using layer-2 sidechains are going to be extremely beneficial for the ecosystem, allowing for quick and easy payments between individuals and businesses.

  

Plasma sidechains may prove to be extremely useful for Tide. By tying in this layer-2 sidechain with Tide and Snowflake (identity management protocol), people could potentially be able to pay with virtually any currency, executing the smart contract with HYDRO on the backend, while the service provider or user receiving the payment receives the currency of their liking.

  

(Note: The Project Hydro community has not yet made any official decisions regarding what scaling systems to incorporate into the Hydro ecosystem)

  

![](https://lh4.googleusercontent.com/xUd2WtbAykaIK2bjqy5P0d-tHp73OqbI2q9LbIF7f-ptmHohWt52EnnUan3UqPf_Q4ZghKHChG8zwC_V9XTg3HyH0SG5Pd-LUwC0Pz6Cxn6O2z-dQejEzxBN0vw1SgJfru8w4ifp)

  

Figure 1: Example of what a layer 2 sidechain integration might look like, using the [Wanchain](https://wanchain.org/) cross-chain connectivity platform.

  

Protocols like [Uniswap](https://uniswap.io/) are also beneficial to the Tide ecosystem. When conducting P2P payments, users will be able to receive payouts in [$DAI](https://makerdao.com/en/dai) (an Ethereum based stablecoin). An example of this is the [Snowmo](https://snowmo.io/) dApp, which was built using Snowflake and ERC-1484. This type of dApp can be built for any type of service provider, whether e-commerce or a brick and mortar store doing POS (point of sale) payments. This enables payment in HYDRO tokens, while the service provider receives DAI automatically.

  

While it might not look like a payment scalability solution, the Hydro-Chainlink partnership has immense potential in regards to Tide, allowing for large payments to be completed within the Hydro ecosystem. By using Chainlink and their oracle smart contracts, users are able to leverage additional security when transacting funds. For example, users would be able to secure HYDRO inside of a smart contract, with Hydro Raindrop 2FA providing a second layer of authentication to blockchain transfers, without requiring the use of a private key [17].

  

## Native Mobile QR Codes and NFC

------------------------------

  

The open-source nature of the Hydro ecosystem means that smartphone manufacturers and app developers will be able to integrate secure, Tide-based payment systems into mobile platforms. With this integration, QR codes, and NFC will allow fast payments in much the same way as Apple Pay and Android Pay work now.

  

The open framework will make it easy for apps, such as social media apps, to integrate Tide payments solutions. By linking your Snowflake to your favorite social media account, instant payments between friends will be as simple as Apple Pay and Google Pay.

  

# Risks

=====

  

The predominant risk facing Tide is Ethereum scaling. This is not such an issue with the Raindrop, Ice, and, to some extent, Snowflake phases of the Hydro roadmap. Those 3 phases are more reliant on reading off the blockchain and the transactions are infrequent, making users likely to want to make the tradeoff between cost and security of completing actions on-chain. However, Tide as a payment protocol will involve many frequent transactions that may incur unacceptable transaction costs if scaling does not occur. On small transactions, these fees act almost as an extra sales tax to users, discouraging crypto payment adoption.

  

The Project Hydro team has implemented disruptive new technology into ERC-1484 and the Hydro P2P beta app to combat these risks. Much work has been done to integrate meta-transaction infrastructure, to provide the opportunity for fee-less everyday payments.

  

Although not currently necessary, it is anticipated that Hydro will use a sidechain, a DPoS chain, Serenity, or some other solution to deal with any scaling issues that may arise. We are watching all developments and solutions carefully to make sure that we are prepared for any eventuality.

  

There is also a risk associated with the reliance on third-party technologies, such as Plasma or Sharding, in dApps built on top of the Hydro Tide protocols. If these technologies break down or become obsolete, then it would be essential to have a backup solution that can be implemented rapidly.

  

# Conclusion

==========

  

The decentralized Web 3.0 has the potential to build on previous technologies, bringing huge benefits to online P2P, B2B, and P2B payments systems

  

In this paper we have seen the three core aspects of Tide:

  

1.  Security: The immutability of the public blockchain, combined with Hydro technology, allows for the addition of an unprecedented level of security to the storage and transfer of funds.

  

2.  Identity: Linking Hydro Tide to our ERC-1484 identity standard creates infrastructure to handle subscriptions, remittance, coupons, and other payment options that were previously not available.

  

3.  Flexibility: Hydro technology allows multiple addresses and currencies to be interlinked, making on-boarding and payments more scalable

  

When solutions such as Plasma take off, and native phone wallets become prevalent, payments using blockchain technology will quickly become mainstream. Hydro Tide, and the Hydro smart contracts associated with it, will be the foundation for the Web 3.0 payments revolution.

  

# Sources

=======

  

1.  <http://www.hit.bme.hu/~buttyan/courses/BMEVIHIM219/2009/Chaum.BlindSigForPayment.1982.PDF>

  

2.  <https://www.forbes.com/forbes/1999/1101/6411390a.html#6b94f113715f>

  

3.  <https://venturebeat.com/2012/10/27/how-ebays-purchase-of-paypal-changed-silicon-valley/>

  

4.  <https://techcrunch.com/2019/04/17/stripe-acquires-touchtech-updates-apis-to-prep-for-strong-customer-authentication-in-europe/>

  

5.  <https://www.statista.com/statistics/274774/forecast-of-mobile-phone-users-worldwide/>

  

6.  <https://www.alliedmarketresearch.com/mobile-payments-market>

  

7.  [https://www.google.com/url?q=https://www.thebalance.com/u-s-retail-sales-statistics-and-trends-3305717&sa=D&ust=1556617308550000&usg=AFQjCNGtatOhOPzr0IPpT2ytcTzjSOuu1Q](https://www.thebalance.com/u-s-retail-sales-statistics-and-trends-3305717)

  

8. <https://blog.continentalcurrency.ca/fx101-remittances/> 

  

9.<https://www.academia.edu/25531594/FACTORS_WHICH_DRIVE_INFLOWS_OF_REMITTANCES_INTO_DEVELOPING_COUNTRIES_CASE_OF_AFGHANIATAN>

  

10. <https://www.hindustantimes.com/business-news/india-highest-recipient-of-remittances-at-79-billion-in-2018-world-bank/story-nT7jLMZBydpyoBCtEfMUfP.html>

  

11. <https://www.worldbank.org/en/news/press-release/2019/04/08/record-high-remittances-sent-globally-in-2018>

  

12. <https://en.wikipedia.org/wiki/Counterfeit_money>

  

13. <https://github.com/ethereum/EIPs/issues/1495><https://gomedici.com/gift-card-fraud-part-of-a-growing-trillion-dollar-global-epidemic/>

  

14. <https://github.com/HydroBlockchain/hcdp/issues/254>

  

15. <https://www.fdic.gov/bank/historical/crisis/overview.pdf>

  

16. <https://gomedici.com/gift-card-fraud-part-of-a-growing-trillion-dollar-global-epidemic/>

  

17. <https://medium.com/hydrogen-api/hydrogen-partners-with-chainlink-fc058a3fd477>



  

General

  

<https://plasma.io/plasma.pdf>

  

<https://docs.uniswap.io/>
