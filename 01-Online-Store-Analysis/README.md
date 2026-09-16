# Online Store Analysis

**Dataset:** 1,200 e-commerce orders  
**Period:** Sept 14-15, 2024 (Day 1-2)  
**Status:** 🔄 Active

---

## 📊 Dataset Overview

- Orders: 1,200
- Customers: 1,189 (unique)
- Products: 7
- Revenue: ₹12,64,762
- AOV: ₹1,054

---

## 🎯 Questions Answered

**Day 1:**
1. What's the total revenue and AOV?
2. How many unique customers vs total orders?
3. Which products generate most revenue?
4. What's the order status breakdown?
5. Why does Chair outperform despite lower pricing?

**Day 2:**
6. Which payment methods are most popular?
7. What's the revenue difference between Credit and Debit Card?
8. How many high-value orders (>₹2000) were delivered?
9. Which referral source drives most orders?
10. What patterns exist in customer IDs and tracking numbers?

---

## 🚨 Key Findings

### 1. Cancellation Crisis
- **Cancelled:** 250 orders (20.83%)
- **Delivered:** 231 orders (19.25%)
- **Impact:** More orders cancelled than delivered!
- **Revenue lost:** ₹2,63,000

### 2. Payment Method Insight
- Credit Card: 234 orders, ₹2,63,848 revenue
- Debit Card: 232 orders, ₹2,32,361 revenue
- **Gap:** ₹31,487 with nearly same order count
- **Reason:** Credit Card AOV = ₹1,127 vs Debit ₹1,001

### 3. Product Performance
- **Winner:** Chair (₹1,95,620)
  - Avg qty/order: 3.16 (bulk buying)
  - Total units: 562
- **Underperformer:** Phone (₹1,51,722)
  - Highest price (₹375) but lowest volume
  - Avg qty/order: 2.63

### 4. Customer Retention Crisis
- Repeat customers: Only 11 out of 1,189 (0.9%)
- Even ₹2,500+ spenders don't return

### 5. Referral Source
- Email: 250 orders (20.8% of total)
- AOV: ₹1,047 (in line with average)

---

## 💡 Recommendations

1. **Immediate:** Investigate cancellation root causes
   - Check: Payment method correlation
   - Analyze: Shipping delays by region
   - Target: Reduce to <10% in 90 days

2. **Product Strategy:**
   - Replicate Chair's bulk-buying success (bundle deals)
   - Fix Phone volume problem (family packs, B2B sales)

3. **Customer Retention:**
   - Loyalty program for 2nd purchase
   - Target: 0.9% → 5% repeat rate

4. **Payment Optimization:**
   - Push premium products to Credit Card users
   - Expected lift: +₹50K if 20% of Debit users switch items

---

## 🛠️ SQL Concepts Used

### Day 1
- SELECT, WHERE, LIMIT
- COUNT, SUM, AVG, MIN, MAX
- COUNT(DISTINCT)
- GROUP BY (single & multi-column)
- ORDER BY DESC/ASC
- ROUND() for formatting

### Day 2
- BETWEEN (range queries)
- IN / NOT IN (multiple values)
- LIKE with wildcards (%, _)
- AND, OR operators
- Complex WHERE conditions
---

## 📅 Daily Progress

### Day 2 (Sept 15)
- ✅ BETWEEN operator (price ranges)
- ✅ IN operator (payment methods, products)
- ✅ LIKE pattern matching (CustomerID, TrackingNumber)
- ✅ Credit vs Debit insight
- ✅ High-value delivered orders analysis

### Day 1 (Sept 14)
- ✅ Environment setup (SQLite, 1200 orders)
- ✅ Basic queries (SELECT, WHERE, COUNT)
- ✅ Aggregations (SUM, AVG, GROUP BY)
- ✅ Cancellation crisis discovered
- ✅ Product performance decomposition


---

**Tools:** SQLite, DB Browser  
**Skills:** SQL querying, business analytics, data storytelling
