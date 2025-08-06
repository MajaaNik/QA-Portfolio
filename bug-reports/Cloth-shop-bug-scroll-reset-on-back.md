# 🐞 Bug Report Summary: Returning from product page resets scroll position and loaded product state in Cloth Shop

**Project:** Maja Nikolic  
**Reporter:** Maja Nikolic  
**Type:** Bug  
**Priority:** Medium  
**Severity:** Medium  

--- 

---

## 📝 Description

On the Cloth Shop **“Haljine”** category page, the user scrolls down until it shows `800 of 831 products loaded`.  
After clicking the **“Vise proizvoda”** (Load more) button, all `831 of 831` products are displayed.

However, when the user clicks on any product near the bottom to open its detail page, and then clicks the **Back** button, the scroll position is reset — the user is taken back to the **top of the page**, and the list again shows only `800 of 831` products, requiring the user to click “Vise proizvoda” once more.

---

## 💻 Environment

- Device: Desktop  
- OS: Windows 10  
- Browser: Chrome  
- Version: 138.0.7204.184 (Official Build) (64-bit)

---

## 🔁 Steps to Reproduce

1. Open the Cloth Shop “Haljine” category page  
2. Scroll down until it shows: `800 of 831 products`  
3. Click on “Vise proizvoda” (Load more)  
4. Click on any product near the bottom to open its detail page  
5. On the Product page, click the browser **Back** button  
6. The scroll position resets; the user is returned to the **top** of the page, and only `800 of 831` products are visible again

---

## ✅ Expected Result

The user returns to the **same scroll position** on the “Haljine” category page with **all 831 products** loaded and visible, **without needing to click** the “Vise proizvoda” button again.

---

## ❌ Actual Result

The user is returned to the **top of the page**, where only `800 of 831` products are loaded.  
User must again click **“Vise proizvoda”** to see the rest.

---

**Priority:** Medium  
**Severity:** Medium

