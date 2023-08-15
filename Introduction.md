# Introduction 

Credentials are a foundational aspect of modern society in that they are the way to identify parties, build trust in transactions and thus supporting the essential workings of nations and global markets (The European Union Blockchain Observatory and Forum, 2019). Credential verification is the process of proving that someone is who they claim to be and that individuals qualifications and certifications are genuine (DIACC, 2020). To have a better understanding of the challenges of the credential verification process, this document will utilize an example use case to illustrate the age verification of a subject.



This use case, known in this document as Use-Case-AV, presents an age verification scenario required to purchase alcohol at a store in Ontario, Canada: 

Ben is a 19-year-old teenager and he is excited to buy his first 12-pack of beer. Ben can decide if he will buy the 12-pack beer either in a physical location or in an online store. In both scenarios he must demonstrate that he is at least 19 years old. To do the verification Ben must present a valid identification that is current, government-issued, and includes his photo and birth date. Some of the acceptable documents include: Ontario Driver’s License, a Canadian passport, a Canadian Citizenship Card, among others (Alcohol and Gaming Commission of Ontario, 2019).

To analyze the current challenges of credential verification, we describe briefly the verification of physical and digital credentials. 



Physical credential verification, although extensively used in transactions, has some challenges due to it being time consuming, bureaucratic, and costly for the credential owner and the issuer organization (O'Donnell, 2016). Also, this verification can be negatively impacted if the physical credential is falsified, as the only way to check its authenticity is to contact the issuing organization directly, which could be challenging in some cases (O'Donnell, 2016). In addition, when a subject (person, place or thing) presents its credential, the verifier has access to all the information in the credential, which in many cases is not necessary; this can result in the low level of privacy of the subject’s information. 

Following the Use-Case-AV, Ben had two options to buy the beer in a physical location or an online store. To illustrate the verification process using a physical credential, we assume that Ben decided to go to a local store. As Figure 1 illustrates, Ben must have a physical document that previously was issued by the government, in this case his driver’s license. Then, the cashier has to verify and trust that the Ben’s license is authentic or communicate with the corresponding entity to validate its authenticity, which can be difficult and time consuming. Finally, when Ben presents his driver’s license, he is presenting more information than just his birth date. For example, Ben is sharing his address, driver’s license number, complete name, and license’s expiration date. Although it looks like something of low importance for some people, sharing this information could negatively impact the privacy of Ben. For example, the cashier can have access to his address and register Ben in a program to receive flyers of store’s promotions without his permission, resulting in an invasive situation.



Digital credentials are fragmented today with limited interoperability, few standards, and they are insecure considering the constant reports of hacks and data breaches that happen every day (The European Union Blockchain Observatory and Forum, 2019). In addition, digital credential verification presents the following concerns. 

- First, having to register and sign up to every online service is inconvenient for a subject because it is required to manage multiple user-password combinations. As reported by NordPass, the average person can have up to 100 passwords to manage with many being using the same passwords for different accounts along with intentionally using easy-to-guess passwords (Rowe, 2021). According to the Identity Theft Resource Center, only 15% of people use unique passwords for different accounts and 85% of people admit to reusing passwords on multiple sites (Turner, 2021). The combination of easy-to-guess passwords and password reuse can be a perfect situation for being vulnerable to hacker attacks and leak of personal information. As Verizon reported, 80% of the data breaches can be attributed to stolen credentials (user-password combination) (DBIR Team, 2020) .

- Second, the online services registration requires the subject to provide personal information that can be stored in multiple servers without any control of its future use. As a result, the subject’s privacy can be compromised directly (O'Donnell, 2016) increasing the risk of data breaches and surveillance. According to the IBM Cost of a Data Breach Report (Cost of a Data Breach Report 2021), the total cost of a data breach in Canada increased 20% from US$4.50 millions in 2020 to US$5.40 millions in 2021 (IBM Security Team, 2021). Some examples of data breaches or hacked systems that have impacted personal information include:

- - The Identity Theft Resource Center recorded 1,339 data breaches impacting over 170 million records in the U.S. in 2017 alone (Gunther & Dickinson, 2018). 
  - In March 2021, the personal information of over 500 million Facebook users from 106 countries was stolen; this information included full names, locations, birthdates, and facebook IDs (Holmes, 2021).
  - More than 40 million records were lost of former or prospective customers of T-mobile who applied for credit with the company. This data breach exposed the names, birth date, social security numbers, and driver's license of the customers (Krebs, 2021)

- Third, the verification of the credential is dependent on the availability of the online services (O'Donnell, 2016). 
- Fourth, the use of Identity Providers such as Facebook and Google to verify a subject's identity can result in the traceability of habits, interests, and other information of the subject resulting in the loss of its privacy (O'Donnell, 2016). 
- Finally, the information used for verification usually is stored in a centralized storage, putting at high risk the personal information of the subjects, and the storage becoming a target for hackers, losing the subject’s trust in the verifier (O'Donnell, 2016). According to the Web Forum organization report, the majority of Americans feel as if they have little control or no control over data collected by companies (81%) and the government (84%) (Hori, 2021). In the same report, it is expressed that Americans are concerned about how the collected data is used by companies (79%) and the government (64%). 

Before continuing with the description of the digital credential verification for our Use-Case-AV, it is relevant to describe some of the methods used today for age verification.

 

- Verification checks. This method relies on customers to confirm their age without any information verification. The customer has to register his information in a website’s form and create a user-password combination. During the registration, the customer has to confirm in a form’s checkbox that they are of the legal age to purchase a controlled product (Marley, 2020). This is a pretty common method of verification that can result in the management of multiple combinations of user-passwords by the customers and low verification levels by the stores.
- Match between credentials and purchase’s information. The verification is executed using security software that will match information between a scanned credential and the purchaser's information (e.g. address of the client and birth date) to ensure that the customer is of the legal age to purchase a controlled product. Also, the software makes use of facial recognition to match a subject’s selfie (a real-time client’s photo) with the picture of the scanned credential. Although this method can be more effective than the verification checks method, the customer has to share a lot of personal information that can result in a high risk for the customer’s privacy. Often these services share the scanned ID and picture with a 3rd party for verification. 

- Double checking during the product’s delivery. This method is a combination of the verification checks and the verification of a physical credential during the product’s delivery. The verification is performed by the delivery agent who completes a visual age verification. If the receiver appears under the legal age, the agent can request the physical credential to confirm the age and a signature to finish the delivery process. This method could be pretty effective for the double check; however, the privacy of the customer is at risk because they are presenting their credentials with all the information to the agent. 



Following the Use-Case-AV, we assume that Ben decided to buy the beer in an online store and the digital credential verification will use the second method described previously. As Figure 2 depicts, Ben has to include his information (e.g. birth date, address, driver’s license number, and a real-time picture) and his scanned driver’s license. Then, a system matches the information to verify if Ben has the legal age to buy the beer. Although this technical solution could be widely used, there is a high risk with the privacy of Ben’s information due to the use of centralized databases that can be easily hacked, so his information could be at risk to be shared with other providers or used by hackers to do fraudulent actions. 



As explained in the previous descriptions, the credential verification process currently faces important challenges that include the need to

- Reduce the exposure of information that is not required for the credential verification and enhance the privacy of the digital credential ecosystems for the different sectors of the economy.

- Establish new solutions to verify the credentials based on the concept of decentralized identities. As a result, the user is the center of the solution and the requirement of third parties is removed. 

- Focus on transparency regarding use and disclosure of personal information.

- Build the trust of the online environments that enable secure and private interactions between the service providers and customers.

  

To respond to the current challenges of the verification process of verifiable credentials, this project describes the VeriDID Verifier . VeriDID Verifier is an open-source technological solution that uses the Self-Sovereign Identity (SSI) approach to verifiable credentials (Citation). SSI gives to a subject the control of generating and managing their credentials in a peer-to-peer decentralized manner (without depending on third-party providers to store and centrally manage the information), enhancing the privacy, transparency, access, and security in transactions (The European Union Blockchain Observatory and Forum, 2019; Folkendt, 2022). Also, SSI reduces the amount of information exposed in presenting a credential and the limit of duration for which the information is shared. In the ecosystem of SSI, a credential is known as a verifiable credential. According to W3C, “a verifiable credential is a tamper-evident credential that has authorship that can be cryptographically verified” (W3C Organization, 2022). 

VeriDID, in addition to being portable and interoperable, verifies claims of verifiable credentials while limiting the need to present additional information which supports the enhancement of privacy and transparency. In addition, VeriDID is a fundamental entity to build trust in ecosystems that enable secure and private interactions between service providers and customers. VeriDID has been conceived to respond to the specific concerns related to the digital credential verification that were identified in the Ontario’s Digital Identity Program (Government of Ontario, 2021). This program aims to introduce a cutting edge technology to prove who is a subject while simplifying and assuring the access to online and in-person services offered by the Government of Ontario (Government of Ontario, 2021).

A project like VeriDID can respond to the current needs about digital credentials expressed by Canadians. According to a survey from the Digital ID and Authentication Council of Canada (Choi, 2022), eight-in-ten Canadians support digital credentials while searching for more control over their own data. Another conclusion is that 91% of the Canadians consider they should have access to the personal data collected about them by the federal government and provincial government. Also, it was identified that 4 in 5 Canadians consider that it is really important that the federal government move quickly to enable a safe and secure digital ID. VeriDID supports identity credential wallets used to hold a verifiable credential, according to the survey, 54% of Canadians are somewhat familiar with the concept of a digital wallet, which could be an advantage for the usability and learning curve to use VeriDID.

The initial version of VeriDID is aimed at verifying credentials issued by the provinces of Ontario, Quebec, and British Columbia. The goal is to provide a system that is better aligned with how an organization would actually use this technology in their regular operations. Current offerings in this marketplace are designed as demonstrations of the technical abilities of Hyperledger Aries technology. We need to review all aspects of the system from the point of view of a user who will work with it every day.

The VeriDID system encompasses several applications

- VeriDID Verifier

- VeriDID Portable

- VeriDID Mobile

- VeriDID Demo

- VeriDID Mediator

- VeriDID Test Network

  

![img](https://lh3.googleusercontent.com/OGsudCOsYXIs4cubFmQU0_9rvg7PBLvZvYcBFKFCngtCogvg5kjLcR5B8OWUOXPdDdeQZUzFjOa9-PRG4innT2C9eUUR6_N0SyRIRG4HRE0S5TAMasP2fpIOhLGEgzADw28yR_OATD_ffc3jpwZsDRg)

Figure 3. High level architecture view of VeriDID



As Figure 3 displays, VeriDID Verifier consists of a set of components that include the channels (web, tablet, and mobile) to interact with the final users, algorithms to execute the verifiable credential verification, a connection with the ledger of blockchain to validate credential information avoiding the centralized control of the information, and a database to store information of the verification maintaining the transparency, privacy, and security.

Following the Use-Case-AV, the Figure 4 illustrates a comparison of the way that VeriDID solves the current challenges presented in the digital credential verification. 





# Self-sovereign identity (SSI) - Big Picture

I suggest to respond to questions such as:

- What is SSI? There is a brief description in the introduction, please check it to avoid confusion.

- How is Blockchain used in SSI?

- Describe that a DID is unique

- According to W3C (W3C Organization, 2022), the roles involved in the verification process of verifiable credentials in SSI include: issuer, verifier, subject, and holder. Describe the integration between these roles and maybe include an image to have more clarity about the connection.
- Use the Use_Case_AV to present the lifecycle of the SSI (issuer, holder, verifier)
- Explain that for VeriDID, a verifiable credential contains: Metadata, claim and signature (meeting 06-14-2022).
- Explain that the verifiable credential is cryptographically signed 

Self-Sovereign identity (SSI) as a philosophical concept has been around for quite some time. The concept of self-sovereign identity (SSI) has been around for more than a decade. However, the ideas and principles underlying SSI have roots in earlier work on digital identity and decentralized systems, some of which go back decades as computer scientists toyed with the idea of a digital identity systems. The growing concerns about digital privacy, data breaches, and the centralization of personal data prompted the exploration of alternative identity models. SSI builds upon the concept of decentralized identity, which was discussed in various forms before the term "self-sovereign identity" was coined.

Self-sovereign identity (SSI) is a digital identity model and philosophy built around the concept that individuals should have full control over their personal data and how it is shared. It allows users to create, manage, and authenticate their own identity credentials without the need for central authorities or intermediaries. SSI leverages decentralized, blockchain-based technology to ensure privacy, security, and user autonomy, enabling individuals to selectively disclose specific information for various purposes while maintaining anonymity and reducing the risk of identity theft or data breaches. Blockchain technology is the best used for SSI systems for several key benefits: 

- Decentralization: In traditional identity systems, personal data is often stored in centralized databases controlled by various organizations, making it vulnerable to hacking and unauthorized access. Blockchain, on the other hand, operates as a distributed ledger, where identity information is stored in a decentralized network of nodes. This removes the need for a central authority to manage identities and reduces the risk of a single point of failure.
- Immutability: Once data is recorded on the blockchain, it becomes extremely difficult to alter or tamper with. Each identity credential or attribute is stored as a transaction on the blockchain, and this transparent and immutable nature enhances the security and integrity of the identity information.
- Privacy and Consent: SSI allows individuals to selectively disclose specific attributes of their identity to different parties, ensuring that they maintain control over their personal information. Blockchain enables cryptographic protocols and zero-knowledge proofs, which allow users to prove the validity of their attributes without revealing the actual data. 
- Interoperability: Different SSI solutions and identity providers can use the same blockchain standards and protocols, fostering interoperability among various systems. This ensures that users can use their self-sovereign identities across multiple applications and services without having to create new identities for each one.
- User Ownership: With SSI on the blockchain, users hold the private keys to their identities and control access to their data. This user-centric approach gives individuals ownership and control over their digital identities, reducing reliance on third parties for identity verification.

When operating all of these essential components are what makes SSI systems so efficient with allowing users fuller control of their information. The system more specifically works through three essential concepts. That of Issuers, Holders and Verifiers.

These three roles make up the core functionality on how an SSI system will operate. While there can be many variations on how an SSI system may run they will inevitably require functionality of these three components.

Issuers: entities that issue verifiable credentials or identity attributes to individuals. These credentials can be anything from a driver's license, educational degrees, or membership certificates. In the SSI model, issuers cryptographically sign these credentials using their private key, ensuring their authenticity and integrity. Once issued, the credentials are stored in the individual's digital wallet.

Holders: individuals who receive and hold the verifiable credentials in their digital wallets. The wallet is an application or system that securely stores and manages the individual's identity data, including the verifiable credentials issued by different issuers. The credentials are cryptographically protected, and the holder has complete control over their wallet and the data it contains. When interacting with verifiers, holders can choose which credentials to share and what information to disclose, ensuring privacy and control over their identity.

Verifiers: entities that need to verify certain identity attributes of the individual during a transaction or interaction. These could be service providers, employers, or any other party that requires proof of specific information about the holder. Instead of requesting a complete identity profile or relying on a centralized identity provider, verifiers can request specific verifiable credentials from the holder. The holder, using their digital wallet, can then present the relevant credentials to the verifier.

When applied to Use_Case_AV we can see how these three core entities function. Ben who wished to purchase the beer had to present a identification document. In this regard he is the Holder of the verifiable credential (his drivers license). The government would serve as the Issuer as they were the foreign entity that gave Ben initial access to his identification that he is now using in this scenario. The Verify is the store owner that will verify Bens information using his verifiable credentials. In this regard the store will accept that the identification is correct from issuers approval of the Identification. While in theory this system lives up to the basic tenants the Issuer, Holder and Verifier relationship (also know as the “Trust Triangle”), it is not fully compatible with the principle of SSI as mentioned previously in this documentation as the Holder does not have proper control over their private information. Nor does this system as presented make use of of any Inoperable system for private information storage and handling.

# ![img](https://lh6.googleusercontent.com/OQR33eAYjC_Za9XrWZ0LnEX-MZ-d5i9qVfaCtNsJ-Fos4MMPYiw7ng8nN83ZQtuvR1drPzFrptPzhnUGf4AfJQM9-NkRbfUP5Z8haO-v_O_5Loqt_KfKINZkAPJ5ob-26EkvVsA-BukAY6B1tdLTmQk)

Source of the image: https://www.w3.org/TR/vc-use-cases/#user-tasks

![img](https://lh3.googleusercontent.com/5qA4NGxArilnrz4pg_U-M8Ea99ppcZoKsZ4N8lUWbSRwzNhjt_iUBxPlQm9kWtIFOR6c_F-OO5IJx53n_7EHQvi5Izwc9cohjkIPQ-NodOygR4fsfXbc8I4hJwEmNYnG3vAl4nm_e1SzujVmPh8ztXM)

Example of life cycle of a verifiable credential (Source: https://w3c.github.io/vc-data-model/#what-is-a-verifiable-credential)



# Glossary

This section contains the list of main definitions used in this document.

**Agent:** “When we use the term "agent" in the SSI community, we more properly mean "an agent of self-sovereign identity." This means something more specific than just a "user agent" or a "software agent." Such an agent has three defining characteristics:

- It acts as a fiduciary on behalf of a single [identity owner](https://docs.google.com/document/d/1gfIz5TT0cNp2kxGMLFXr19x1uoZsruUe_0glHst2fZ8/edit#heading=h.2e5lma3u6c9g) (or, for agents of things like IoT devices, pets, and similar things, a single controller).
- It holds cryptographic keys that uniquely embody its delegated authorization.
- It interacts using interoperable [DIDComm protocols](https://github.com/hyperledger/indy-hipe/pull/69).

These characteristics don't tie an agent to any particular verification network. It is possible to implement agents without any use of a verification netowrk at all (e.g., with [peer DIDs](https://github.com/openssi/peer-did-method-spec)), and some efforts to do so are quite active.” (https://github.com/hyperledger/aries-rfcs/blob/main/concepts/0004-agents/README.md)

**Blockchain (Distributed ledger):**

**CANdy network:** A publicly accessible network run by a collection of Canadian provincial governments used for verifying the cryptographic claims stated in the verifiable credentials that they have issued.

**Claim:** “An assertion made about a subject.” (W3C Organization, 2022)

**Credential:** “A credential is an attestation of qualification, competence, or authority issued to an entity (e.g., an individual or organization) by a third party with a relevant or de facto authority or assumed competence to do so. Examples of credentials issued to people include a driver’s license, a passport, an academic degree, and so on. Credentials are also issued to companies, such as business registrations, building permits, and even health inspection certifications.” (Curran, 2021). “A set of one or more claims made by an issuer” (W3C Organization, 2022)

Data breach: “A data breach is any incident in which confidential or sensitive information has been accessed without permission… Breaches are the result of a cyberattack by criminals who gain unauthorized access to a computer system or network. They then steal the private, sensitive, or confidential personal and financial data of the customers or users contained within.” (Sobers, 2022)

**Database: “**database is an organized collection of data stored and accessed electronically.” (https://en.wikipedia.org/wiki/Database).

**Decentralized Identifier (DID)**: “A portable URL-based identifier associated with an entity. These identifiers are most often used in a verifiable credential and are associated with subjects such that a verifiable credential itself can be easily ported from one repository to another without the need to reissue the credential. An example of a DID is did:example:123456abcdef.” (W3C Organization, 2022)

**DID Document:** “Also referred to as a DID document, this is a document that is accessible using a verifiable data registry and contains information related to a specific decentralized identifier, such as the associated repository and public key information.” (W3C Organization, 2022)

**Digital credential:**

**Digital identity wallet / credential repository?:**

**Entity: “**A thing with distinct and independent existence, such as a person, organization, or device that performs one or more roles in an ecosystem.” (W3C Organization, 2022)

**Hyperledger Aries:**

**Holder:** “A role an entity might perform by possessing one or more verifiable credentials and generating verifiable presentations from them.Example holders include students, employees, and customers.” (W3C Organization, 2022)

**Issuer** (known also as Identity Service Provider): **“**A role an entity performs by asserting claims about one or more subjects, creating a verifiable credential from these claims, and transmitting the verifiable credential to a holder. Example issuers include corporations, non-profit organizations, trade associations, governments, and individuals.**”** (W3C Organization, 2022).

**Physical credential:**

**Self-Sovereign Identity (SSI):** 

**Subject:** “An entity about which claims are made. Example subjects include human beings, animals, and things. In many cases the holder of a verifiable credential is the subject, but in certain cases it is not. For example, a parent (the holder) might hold the verifiable credentials of a child (the subject), or a pet owner (the holder) might hold the verifiable credentials of their pet (the subject).” (W3C Organization, 2022)

**Validation:** “A process that confirms the accuracy of digital identity information about a subject as established by an authoritative party.” (DIACC's Trust Framework Expert Committee, 2020) 

**Verification:** The evaluation of whether a verifiable credential is an authentic and timely statement of the issuer. This includes checking that: the credential conforms to the specification; the proof method is satisfied; and, if present, the status is successfully checked. (W3C Organization, 2022)

**Verifiable credential:** “A verifiable credential is a tamper-evident credential that has authorship that can be cryptographically verified. ” (W3C Organization, 2022). Examples of verifiable credentials can be identified in different domains such as education (digital transcript), retail (age verification, address verification), healthcare (insurance claim, prescribing), professional credentials (job applicant), and legal identity (digital driver’s license, refugee crisis) (W3C Organization, 2022).

**Verifier:** “A role an entity performs by receiving one or more verifiable credentials, optionally inside a verifiable presentation, for processing. Example verifiers include employers, security personnel, and websites.” (W3C Organization)

**Zero-Knowledge proof:** “A zero-knowledge proof is a cryptographic method where an entity can prove to another entity that they know a certain value without disclosing the actual value.” (W3C Organization, 2022)

