# ByteBankers
A repsository for the NPCI Hackathon
# Byte Points System

The Byte Points System is a universal loyalty program that allows customers to earn and redeem "byte points" across multiple sellers, creating a unified ecosystem for rewards. This system ensures that sellers can issue loyalty points without incurring loss when customers use points across platforms.

## Overview

In the Byte Points System, each "byte point" is equivalent to 1 rupee. When a seller issues byte points, they pay 1 rupee per point to the system. The key idea is that when points are used, they are converted back into money and paid to the seller where the points are redeemed, ensuring that the seller does not bear the loss of accepting these points.

- **1 Byte Point = 1 Rupee.**
- Sellers pay the system for issuing points.
- Points can be redeemed at any participating seller.
- When points are redeemed at a new seller, they receive the equivalent amount in money.
- When points are used at the original seller, they provide a discount equivalent to the points redeemed, but they receive the same amount of money back.

## How It Works

### 1. Issuing Byte Points
- When a customer makes a purchase at a participating seller, the seller issues byte points corresponding to the transaction amount.
- For example, if a customer spends ₹100, they receive 100 byte points.
- The seller pays the system ₹100 to issue those points (1 byte point = 1 rupee).

### 2. Redeeming Byte Points
- The customer can redeem their points at any participating seller. 
- If they redeem their points at a new seller, the points are converted into rupees, and the new seller receives the money equivalent to the points used.
- If the points are redeemed at the original seller, they offer the customer a discount of ₹100 (if 100 points are used), but the seller receives ₹100 back from the system.

### 3. Seller Benefits
- **For the Issuing Seller:**
  - The original seller benefits from customer loyalty by offering universal byte points. While they may provide a discount when points are redeemed at their store, they receive the same amount back in monetary value, thus ensuring no loss.
  
- **For the Redeeming Seller:**
  - The redeeming seller is assured that accepting points from other sellers will not incur any loss since they will receive the equivalent rupee value when points are redeemed at their store.

- **For the Customer:**
  - Customers enjoy the flexibility to redeem their points across various sellers, increasing the appeal of the loyalty program and encouraging repeat business.

## System Architecture

### Key Components:
1. **Point Issuance System:**
   - Allows sellers to issue byte points when a customer makes a purchase.
   - The seller pays for the points issued, maintaining a 1:1 ratio with rupees.

2. **Point Redemption System:**
   - When points are redeemed, the seller receiving the points is paid the equivalent rupee value.
   - If the points are used at the issuing seller, they provide a discount, but the system reimburses them the same amount.

3. **Transaction Ledger:**
   - All point issuance and redemption transactions are recorded to ensure transparency and integrity.
   - Points cannot be double-spent, and each transaction is logged for audit purposes.

### Security:
- All transactions are encrypted to protect user and seller data.
- Role-based access control (RBAC) is implemented to ensure that only authorized users can issue or redeem points.

## Benefits

- **Customer Loyalty:** Customers are incentivized to remain loyal to sellers who offer byte points, knowing they can use their points across multiple platforms.
- **No Loss to Sellers:** Sellers do not lose money when points are redeemed, as the points are convertible to rupees, ensuring a balanced exchange.
- **Cross-Seller Collaboration:** Sellers can collaborate in creating a unified ecosystem of loyalty, potentially increasing their customer base and sales volume.

## Getting Started

To integrate the Byte Points System into your platform, follow these steps:

1. **API Integration:**
   - Use the provided RESTful APIs to connect your platform with the Byte Points System.
   - API documentation is available in the `/docs` directory.

2. **Setting Up Points Issuance:**
   - Implement functionality to issue byte points during customer transactions.
   - For each transaction, the seller will pay for the issued points, ensuring the correct amount is deducted.

3. **Setting Up Redemption:**
   - Implement point redemption at your store, ensuring customers can use their points for discounts or to pay for purchases.
   - When points are redeemed, ensure you receive the equivalent rupee value back from the system.

## Example

- **Customer Purchase:**
  - Customer spends ₹200 at Seller A.
  - Seller A issues 200 byte points.
  - Seller A pays ₹200 to the system to issue those points.
  
- **Customer Redeems Points at Seller B:**
  - Customer spends 200 byte points at Seller B.
  - Seller B receives ₹200 from the system and provides the customer with the equivalent in products or services.

- **Customer Redeems Points at Seller A:**
  - Customer spends 200 byte points at Seller A.
  - Seller A provides a ₹200 discount but receives ₹200 back from the system.
