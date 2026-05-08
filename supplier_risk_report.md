# Supply Chain Risk Control Tower: Supplier Analysis

Based on the provided dataset, the suppliers have been evaluated using the following criteria:
- **CRITICAL RISK**: OTIF_Score < 85
- **HIGH COST**: Price_Index > 105
- **Regional Risk**: Suppliers in Asia have an elevated risk profile due to longer lead times.

## 🚨 Top 3 Most Risky Suppliers

The following suppliers represent the highest risk to the supply chain based on the compounded risk factors:

| Supplier Name | OTIF Score | Price Index | Region | Risk Flags |
| :--- | :--- | :--- | :--- | :--- |
| **Tech_Components_Shenzhen** | 75 | 112 | Asia | ⚠️ **CRITICAL RISK**, 💸 **HIGH COST**, 🌏 **ASIA** |
| **Asian_Steel_Works** | 82 | 108 | Asia | ⚠️ **CRITICAL RISK**, 💸 **HIGH COST**, 🌏 **ASIA** |
| **Dhaka_Jute_Mills** | 74 | 82 | Asia | ⚠️ **CRITICAL RISK**, 🌏 **ASIA** |

> [!WARNING]
> **Tech_Components_Shenzhen** and **Asian_Steel_Works** both trigger all three risk parameters: they suffer from poor delivery reliability (CRITICAL RISK), are excessively expensive (HIGH COST), and are located in a high-lead-time region (Asia). **Dhaka_Jute_Mills** holds the lowest overall OTIF score in the dataset (74).

## 🛡️ Suggested Mitigation Strategy

To address these vulnerabilities, the following mitigation strategies are recommended:

1. **Immediate Engagement & RCA (Root Cause Analysis)**
   - Initiate immediate performance reviews with the identified suppliers. Demand a corrective action plan (CAP) specifically addressing their low OTIF scores.
2. **Dual-Sourcing / Nearshoring**
   - Given the combined "High Cost" and "Asia" regional risk, begin identifying backup suppliers in the "Europe" region for critical components currently sourced from *Tech_Components_Shenzhen* and *Asian_Steel_Works*. European alternatives present in the dataset (e.g., *Silesia_Fittings*, *Warsaw_Logistics_Hub*) show strong OTIF scores and lower price indices.
3. **Renegotiate or Phase Out**
   - Use the low OTIF scores as leverage to renegotiate the high Price Indexes (above 105). If performance does not improve within a defined quarter, initiate a phased exit strategy to transition volume to more reliable and cost-effective suppliers.
