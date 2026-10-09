# Daigou Receipt Calculator — Showcase Case Study

> From messy shopping orders to clear customer receipts.

**Type:** Standalone browser-based HTML tool (not a packaged Chrome extension).  
**Template:** Use Cases + Before & After  
**Audience:** Japanese shopping proxies, group-buy organizers, small resellers.  
**Source:** https://github.com/COLDDCC/daigou-receipt-calculator

## Hero

**From order spreadsheets to customer-ready receipts.**

Stop manually comparing shopping lists, checking which items were purchased, and calculating each customer's total. Import your registration sheet and actual purchase results to prepare accurate settlements, printable receipts, and a spreadsheet-ready batch summary.

**CTA:** View source on GitHub  
**Secondary CTA:** Open the HTML tool locally

**Visual direction:** A real (not fictional) screenshot of the tool with the receipt result alongside it. Do not invent customer names, amounts, or UI screenshots.

## The problem: two spreadsheets, one complicated settlement

Customers submit their requested items before a purchase, but actual shop orders may contain discounts, unavailable items, differing prices, and shared service or shipping fees. Reconciling everything manually can make customer-facing totals difficult to explain.

## Three key use cases

### 1. Match requested items with actual orders

Paste the **registration sheet** first, containing the customer, requested product, original price and product URL. Then paste the **settlement sheet** from the actual order.

The calculator matches product identifiers where possible, falling back to product names, and separates unavailable items from purchased ones.

**Screenshot brief:** Place “从表格导入” next to “二次核算 · 最终价格核对”; use genuine sample data.

### 2. Calculate what each customer owes

Calculate actual item totals from the settlement sheet, allocate communication fees across purchased item quantities, account for freight charges, choose an exchange rate, and set rounding preferences. Unpurchased items are excluded from the payable total and allocation count.

**Screenshot brief:** Show the fee settings, discounted item and receipt output.

### 3. Generate a clear receipt and batch summary

Download or copy each customer's receipt as a PNG. Generate a tab-separated summary containing customer, quantity, RMB amount, JPY amount and payment-method column for direct paste into Excel or WPS.

**Screenshot brief:** Show the finished receipt and the five-column summary side by side.

## How it works

1. **Paste requested products.** Import your registration sheet, optionally with a customer column to split a batch.
2. **Verify the real purchase.** Paste the shop's final settlement list. The recorded final line amount is used to reconcile discounts and purchased quantities.
3. **Set shared charges.** Configure exchange rate, fees and rounding.
4. **Export results.** Download/copy individual receipt images and paste the batch summary into a spreadsheet.

## Before and after

| Before | After |
|---|---|
| Compare two sheets line by line | Match original requests to purchased items |
| Manually flag out-of-stock goods | Mark unpurchased items and exclude them from totals |
| Calculate fees and currency conversion repeatedly | Apply settings to a batch |
| Type each customer's payment breakdown | Export per-customer PNG receipts |
| Build a new summary in Excel | Copy a ready-to-paste tab-separated summary |

## Key details and accuracy

- Uses the settlement sheet's final **金額** field, rather than applying a blanket discount twice.
- Attempts product-ID matching before name matching.
- Excludes unpurchased items from totals and per-item fee allocation.
- A customer summary can include total RMB, product-only JPY and a blank payment-method field.
- Intended for transparent settlement, not financial or tax advice.

## Trust and platform notes

- The repository currently contains a standalone `index.html`, not a Chrome extension `manifest.json`.
- The README states it works by opening the file in a browser without dependency installation.
- Do **not** display “Install Chrome Extension,” Chrome store ratings, permission claims, or verified-safe badges.
- Public product-page hosting on Extension Gallery is not implemented yet. This case study can serve as structured content and a future public-page fixture.

## Suggested visual assets

1. Hero: screenshot of the imported registration table + finalized receipt.
2. Workflow: screenshot of the purchase reconciliation panel.
3. Calculation: real fee settings and final customer total.
4. Export: PNG receipt and the pasted Excel/WPS summary.

Use real screenshots with anonymized or dummy customer/order information.