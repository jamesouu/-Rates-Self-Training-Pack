# 📘 Week 01 — Bond Pricer  

## 🎯 **Objective**  
Build a simple Python bond pricer for **U.S. Treasuries** and learn the foundations of **linear rates products**.  

This is the first step in replicating the training path of a sell-side analyst on a **Rates Linear Desk**.  

---

## 🧩 **Key Concepts Covered**  
- Time value of money  
- Discount factors and yield-to-maturity (YTM)  
- Price vs yield relationship  
- Duration & convexity (measures of interest rate risk)  
- Curve shapes (steepening, flattening, inversion)  

---

## 🛠 **Mini-Project Deliverable**  
A Python notebook:  
- Inputs: coupon rate, maturity, yield, frequency  
- Outputs:  
  - Clean Price & Dirty Price  
  - Yield-to-Maturity (YTM)  
  - Duration & Convexity  
  - Price/yield curve visualization  

---

## 📂 **Folder Structure**  
```
Week01_Bond_Pricer/
│
├── bond_pricer.ipynb      # Python notebook for bond pricing
├── notes.md               # Written notes & explanations
└── data/                  # Sample UST curve data
```

---

## 📊 **Sample Output**  

- **Price vs Yield Curve** (for a 10Y UST, 3% coupon):  

```text
Yield (%)    Price ($)
2.00         108.98
3.00         100.00
4.00          92.27
```

- **Risk Measures (10Y UST)**  
  - Macaulay Duration: 8.52 years  
  - Modified Duration: 8.26  
  - Convexity: 73.4  

---

## 📖 **Learning Notes**  
- Bond pricing is the **foundation of the rates world**. Every product (swaps, swaptions, exotics) ultimately depends on discount factors.  
- Price is inverse to yield → traders constantly quote both.  
- Duration & convexity → show how bond prices react to parallel shifts in rates (risk mgmt tool).  
- In practice, you’d pull curves from Bloomberg; here we simulate or use FRED datasets.  

---

## 🚀 **Next Steps (Week 02 Preview)**  
- Extend bond pricing into **spread products**.  
- Track **BTP-Bund spread** (Italy vs Germany).  
- Add auction cycle analysis and political risk context.  
