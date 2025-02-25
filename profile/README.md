# Baba Vanga

This project demonstrates a decentralized prediction market built on the native Bitcoin network using Glittr. Our system leverages Automated Market Makers (AMMs) — specifically a Constant Sum Market Maker (CSMM) model — to provide continuous liquidity and dynamic pricing for binary outcome tokens. An off-chain oracle is integrated to resolve market outcomes based on real-world data.

![image](https://github.com/user-attachments/assets/ea3fbbb6-54aa-4e62-a406-c71fa5717290)

## Overview

- **Prediction Market:**  
  Users create markets on questions like "Will Bitcoin reach 125K USD by March?" and mint outcome tokens (YES and NO) to represent the possible outcomes.

- **AMMs (CSMM):**  
  Instead of an order book, our system deploys an AMM based on the CSMM model. With this model, the sum of the outcome prices is always fixed (e.g., $1), so that the price of each token directly reflects the market's estimated probability.

- **Oracle Integration:**  
  At market resolution, an off-chain oracle fetches data (e.g., BTC/USD price) and generates a signed oracle commitment. This commitment is included in the resolution transaction, ensuring that the market outcome is determined by verified external data.

## Protocol Advancements for Custom AMM CSMM

Recent protocol advancements have enhanced our custom AMM CSMM, delivering increased flexibility and efficiency to our prediction market ecosystem. These improvements include:

- **Custom Configuration:**  
  The system now supports customizable parameters for the CSMM model, allowing market creators to adjust fee structures and liquidity parameters to better reflect market dynamics.

- **Enhanced Liquidity and Dynamic Pricing:**  
  The updated protocol introduces improvements in the liquidity mechanism. This ensures a smoother price discovery process with dynamic adjustments that maintain the invariant sum of outcome prices while accommodating varying levels of market participation.

- **Optimized Oracle Integration:**  
  With the revised integration, the off-chain oracle now offers faster and more accurate resolution of market outcomes. This ensures that price feeds (such as BTC/USD) are captured with enhanced reliability and incorporated into market resolutions seamlessly.

- **Robust and Scalable Architecture:**  
  The protocol advancements address scalability and security, providing a more robust framework to support higher transaction volumes and more complex market scenarios. This positions the platform to handle an expanding user base and more diverse prediction market queries.

For detailed technical discussions and implementation specifics, please refer to the following pull requests:
- [Glittr SDK Custom AMM Enhancements](https://github.com/Glittrfi/glittr-sdk-public/pull/3)
- [Glittr Core Custom AMM Improvements](https://github.com/Glittrfi/glittr-core-public/pull/4)

---

## **Deployment & Transactions**
The following links provide direct access to key blockchain transactions relevant to our system:

🔹 **Automated Market Maker Deployment**  
🔗 [View Transaction](https://explorer.glittr.fi/tx/8f7a5602721a4596284f8d639a059a80adcac9e07b3c3b1a06973e3c2e91ecfc)  

🔹 **Liquidity Deposit**  
🔗 [View Transaction](https://explorer.glittr.fi/tx/944ba877cda30862dec1ba1b8223cdb1791616c774cf1174b3047123b311e241)  

---

## **Frontend Integration: Glittr Wallet & Contracts**
The frontend of our prediction market seamlessly integrates the **Glittr Wallet** with the deployed contracts. The following key components handle wallet interactions and contract execution:

🔹 **Navbar Component - Wallet Integration**  
📌 [View Code](https://github.com/babavanga-encode-defi/frontend-app/blob/c1bc1a5f3318fd80ee54e0ef4bd2d720a8268409/src/components/Navbar.tsx#L42)  

🔹 **Create Contract Form - Market Creation Logic**  
📌 [View Code](https://github.com/babavanga-encode-defi/frontend-app/blob/c1bc1a5f3318fd80ee54e0ef4bd2d720a8268409/src/components/CreateContractForm.tsx#L45)  

---

This project continues to push the boundaries of decentralized prediction markets, offering a **scalable, efficient, and user-friendly** platform for market participants. 🚀
