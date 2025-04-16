# Table of Contents
- [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Roadmap](#roadmap)
  - [Mobile Apps & Website](#mobile-apps-website-etc)
  - [Dialogue Section](#dialogue-section)
  - [Voting Section](#voting-section)
    - [Anonymous Voting System](#anonymous-voting-system)
      - [Roadmap](#roadmap-1)
    - [Identity Verification using passport](#identity-verification-using-passport)
    - [Secure Profile Creation](#secure-profile-creation)
    - [Smart Contract Integration](#smart-contract-integration)
    - [Data Security](#data-security)
    - [Anonymous Voting](#anonymous-voting)

## Introduction
The initial model of Iranians.vote consists of two parts: Dialogue and Trustworthy Voting. Trustworthiness includes guaranteeing vote non-repeatability, voter uniqueness, complete protection of voter identity and privacy, and transparency in tallying and finding social choices.

## Roadmap
* Add newsletter, and collaboration infrastructure for the entire platform  
* Playground for familiarization with the processes and testing the games  
* Implement experimental platform in a democracy (goe26) and analyze and publish findings

## Mobile Apps Website etc. 
* [Iranian National Identity Card Assistant](https://github.com/Iranians-Vote-Digital-Democracy/INIDCA) (read card's certificate, version, meta data)
* [Iranians Vote Android App](https://github.com/Iranians-Vote-Digital-Democracy/iranians-vote-android)
* [Iranians Vote iOS App](https://github.com/Iranians-Vote-Digital-Democracy/iranians-vote-ios)
* [Website](https://github.com/Iranians-Vote-Digital-Democracy/iranians.vote)
  
## Dialogue Section
[Nextodon](https://github.com/tcfev/Nextodon) is a social network compatible with Fediverse and Mastodon with additional features that facilitate structured group dialogue. Nextodon provides written discussion capabilities, basic polling features, and a basic infrastructure for crypto economy.

## Voting Section
Digital discussions (from Nextodon or other platforms) can be brought to [Iranians.vote](https://iranians.vote) to find social choices and reach reliable conclusions through polling.


### Anonymous Voting System
Our voting system incorporates a robust privacy-preserving architecture that leverages biometric documents and zero-knowledge proofs (ZKP) to enable secure, anonymous voting while maintaining voter authenticity. We currently support biometric passports. [(ICAO's Doc 9303)](https://www.icao.int/publications/documents/9303_p9_cons_en.pdf)

#### Roadmap
- [Add support for Iranian National ID card](https://github.com/Iranians-Vote-Digital-Democracy/INID/blob/main/README.md)
- Add support for German National ID card (Ausweis)
  
### Identity Verification using passport
- Uses biometric passport data as the foundation for voter authentication
- Validates passport authenticity through digital signatures without exposing personal data
- Employs zero-knowledge proofs to verify voter eligibility while preserving privacy

### Secure Profile Creation
- Generates digital voter profiles using passport biometric data as identifiers
- Creates anonymous digital credentials that can’t be linked to individual voters
- Validates passport authenticity using ZKP technology without revealing personal information

### Smart Contract Integration
- Implements blockchain-based smart contracts for transparent vote recording
- Uses three-contract architecture:
  - Investment contract (INV) for transaction fee management
  - Registration contract (REG) for anonymous voter registration
  - Voting contract (VOT) for anonymous ballot casting and tallying

### Data Security
- All verification happens locally without transmitting personal data
- No personal information is stored or accessible by external parties
- Uses cryptographic techniques to ensure vote secrecy while maintaining verifiability

### Anonymous Voting
- Employs a nullifier-based system to prevent double voting while maintaining anonymity
- Separates registration transactions from voting transactions to prevent correlation
- Allows voters to cast ballots from any device using secure credentials without exposing identity
