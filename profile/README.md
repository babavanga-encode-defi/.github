# Baba Vanga 

This project demonstrates a decentralized prediction market built on the native Bitcoin network using Glittr. Our system leverages Automated Market Makers (AMMs) — specifically a Constant Sum Market Maker (CSMM) model — to provide continuous liquidity and dynamic pricing for binary outcome tokens. An off-chain oracle is integrated to resolve market outcomes based on real-world data.

![image](https://github.com/user-attachments/assets/ea3fbbb6-54aa-4e62-a406-c71fa5717290)


## Overview

- **Prediction Market:**  
  Users create markets on questions like "Will Bitcoin reach 125K USD by March?" and mint outcome tokens (YES and NO) to represent the possible outcomes.

- **AMMs (CSMM):**  
  Instead of an order book, our system deploys an AMM based on the CSMM model. With this model, the sum of the outcome prices is always fixed (e.g., \$1), so that the price of each token directly reflects the market's estimated probability.

- **Oracle Integration:**  
  At market resolution, an off-chain oracle fetches data (e.g., BTC/USD price) and generates a signed oracle commitment. This commitment is included in the resolution transaction, ensuring that the market outcome is determined by verified external data.
