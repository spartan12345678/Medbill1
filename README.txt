MEDBILL V1 - OFFLINE-FIRST PHARMACY BILLING STARTER

WHAT THIS IS
A mobile-first installable Progressive Web App (PWA) prototype. It is NOT a native Android APK and is NOT certified for commercial pharmacy/GST use.

FEATURES IN THIS STARTER
- Local IndexedDB storage on the device/browser
- Medicine batch inventory with expiry date and stock quantity
- Basic FEFO search ordering by expiry
- GST and non-GST billing modes
- Configurable item GST rates (0, 5, 12, 18, 28; custom rates must be verified before use)
- Stock deduction on completed sale
- Invoice history and print/save as PDF using the browser print dialog
- Shop profile settings
- JSON backup export
- Service worker caching for offline app shell after first successful load

IMPORTANT LIMITATIONS
- No cloud sync or Supabase backend is configured yet.
- No backup import/restore UI yet. Keep exported JSON backups safe.
- No purchase register, supplier workflow, returns/credit notes, barcode scanner, split payments, GST return reporting, e-invoice or e-way bill support.
- Tax logic is a starter calculation only. It does not yet handle every Indian GST rule, intra/inter-state tax split, discounts, exemptions, credit notes, statutory invoice fields or legal requirements.
- Invoice numbering is a basic local sequence and needs stronger transaction-safe fiscal-year logic before live commercial use.
- This is not a substitute for qualified GST/pharmacy compliance review. Never use unverified tax rates. Do not store sensitive patient data in this prototype.

HOW TO TEST
1. Serve the folder over HTTPS or localhost. Service workers/PWA installation do not work reliably from a file:// URL.
2. Open index.html through the hosted URL in Chrome on Android.
3. Add shop settings, then add medicine batches in Inventory.
4. Return to Billing, select invoice type, add medicine, and complete a test sale.
5. Check Invoices and Inventory. Use only test/demo data.
6. Use Chrome menu > Add to Home screen / Install app when available.

NEXT ENGINEERING MILESTONE
Add a robust tax engine (CGST/SGST/IGST, place of supply, item-wise rounding), transactional invoice numbering, import/restore, purchase/supplier modules, audit log, automated tests, then secure optional cloud sync.
