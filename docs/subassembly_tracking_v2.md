# Subassembly Tracking v2 User Guide

**Date:** 18-08-2026  
**Contact:** support@factri.ai

---

## 1. Introduction

This guide covers the current (v2) sub-assembly tracking flow used at the Chennai and Bangalore plants. It replaces the per-order flow described in the [Subassembly Tracking Module User Guide](subassembly_tracking.md).

What changed from v1:

- **One standing QR per sub-assembly type.** Each sub-assembly material (for example *Head board assly - 18BBT*) has a single standing order and a single QR code. Scan the same QR every time you build one; there are no per-chassis sub-assembly orders and no repeated QR printing.
- **One production stage: Move to Stock.** Building a sub-assembly is recorded as a single confirmation.
- **Chassis linkage at confirmation.** While confirming, you select the **SO Number** (sale order) and the **SF Number** (chassis) the sub-assembly belongs to. The system uses this to show, for any chassis, which sub-assemblies are already built.

---

## 2. Scanning a Sub-Assembly QR

1. Open the app and tap **'SCAN QR/BARCODE'** on the landing page.
2. Scan the QR code of the sub-assembly type you built. The standing order page opens, showing the material name and the **Production Stages** list with **Move to Stock**.
3. Tap **Move to Stock** to open the confirmation form.

---

## 3. Confirming a Sub-Assembly (Move to Stock)

Fill the confirmation form:

1. **Defect Code**: select **PASS (PASS)** for a good part.
2. **Job Notes**: optional remarks about this build.
3. **SO Number**: select the sale order the sub-assembly is for.
4. **SF Number**: select the chassis SF number under that sale order. The list offers only chassis that do not already have this sub-assembly; SF numbers under an active quality block do not appear.
5. **Supervisor**, **Contractor 1**, **Contractor 2**: select from the dropdowns.
6. Attach a photo using **'Upload'** or **'Camera'** (capture with **'Capture Photo'**).
7. Tap **'Confirm'**. A success message appears and the entry is recorded with the current date and time.

To record several of the same sub-assembly one after another, scan the same QR again and repeat.

<!-- VIDEO-ID-PENDING: subassembly-tracking-v2-01.mp4 -->
<iframe src="https://drive.google.com/file/d/VIDEO-ID-PENDING-01/preview" width="711" height="400" allow="autoplay; fullscreen" allowfullscreen="true" frameborder="0"></iframe>

---

## 4. Viewing a Chassis's Consumed Sub-Assemblies

To check which sub-assemblies are already built for a chassis:

1. Tap **'Search order ID or details...'** on the landing page and search by the SO or SF number (for example *6529-1*).
2. Open the chassis order (the entry that shows the SF number, for example *2026SF53674C || 2526006529-1*).
3. Open the **Consumed Sub-Assemblies** view. It lists every sub-assembly already built for that chassis with its **SO Number**, **Qty** and **Confirmed At** time. A sub-assembly confirmed a moment ago appears here immediately.

<!-- VIDEO-ID-PENDING: subassembly-tracking-v2-02.mp4 -->
<iframe src="https://drive.google.com/file/d/VIDEO-ID-PENDING-02/preview" width="711" height="400" allow="autoplay; fullscreen" allowfullscreen="true" frameborder="0"></iframe>

---

## 5. Dashboard and Daily Report

On a desktop browser:

1. Click the **'View PPC Dashboard'** button on the landing page and select the **Sub Assembly** tab at the top right.
2. **Daily Sub Assembly Trend** shows the day-wise build counts for the selected plant and month.
3. **Daily Sub Assembly Report** lists every confirmation with Report Date, Shift, Time, Chassis No / WO, FG No., SO Number, SF Number and Description. Click a date on the trend chart to filter the report to that day.
4. Use the column filters or the search box to narrow the list, and **'Export XLSX'** to download it.

<!-- VIDEO-ID-PENDING: subassembly-tracking-v2-03.mp4 -->
<iframe src="https://drive.google.com/file/d/VIDEO-ID-PENDING-03/preview" width="711" height="400" allow="autoplay; fullscreen" allowfullscreen="true" frameborder="0"></iframe>

---

## 6. Notes

- The same sub-assembly QR is reused indefinitely; print new QR sheets only when adding a new sub-assembly type.
- If an SF number is missing from the SF Number list, it either already has this sub-assembly recorded or is under an active quality block. Contact your supervisor to review blocked SF numbers.
- Entries are permanent. If a confirmation was made with the wrong chassis, contact support@factri.ai to correct it.
