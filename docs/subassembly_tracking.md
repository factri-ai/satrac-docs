# Subassembly Tracking Module User Guide

**Date:** 22-09-2025  
**Contact:** support@factri.ai

---

## 1. Introduction
This document outlines the guidelines for using the DataWiz application in the Bangalore and Chennai plants for the Subassembly Tracking use case.

---

## 2. Installation and Login
The application URL is [https://satrac.datawiz.app](https://satrac.datawiz.app). Chrome is the recommended browser.

For mobile app installation, please refer [this section](production_tracking.md#2-installation-and-login).

---

## 3. Printing Chassis QR Codes
To print QR codes for chassis orders released to the Chennai or Bangalore plants:

1. Login to the app on a **Desktop** device.
2. From the orders table select the Subassembly orders section on the landing page, you will see all the subassembly orders auto-generated in the system.
3. Select the **checkboxes** for the required orders. Use the filter options or increase the "per page" value to select multiple orders. You can also use the Sale Order column filter option to filter only the required subassembly orders.
4. Select the **‘Print QR’** option to download a PDF containing the unique chassis QR codes.

<iframe src="https://drive.google.com/file/d/1LapwsqpRuPPB5aXEaOkIJlThpfNlr7So/preview" width="711" height="400" allow="autoplay; fullscreen" allowfullscreen="true" frameborder="0"></iframe>

---

## 4. Scanning and Making Confirmations
The following actions can be performed to capture production data:

* **COMPLETE:** Press when work is finished to capture completion time and input details like line number and supervisor.

<iframe src="https://drive.google.com/file/d/1_Wi-A6u4HsnTXS3fCMdci4_0ZYs1UeIC/preview" width="711" height="400" allow="autoplay; fullscreen" allowfullscreen="true" frameborder="0"></iframe>

---

## 5. Subassembly Consumption
The completed subassemblies can be consumed/linked with the SF numbers. Follow the below steps to do the same:

1. Open the **SUBASSY** stage completion form of a SF number.
2. As you scroll down you will see certain **Subassembly item codes** and available dropdowns for them.
3. Click on the right most **scan button** for any of the subassembly item, and scan the **QR code of the Subassembly order** that was consumed for this specific SF number (which should be attached to the subassembly in question). In case an **invalid** (incompete or subassembly order for an different SF number) subassembly order QR code is scanned, the system will not accept the same.
4. You can also **click on the dropdown**. A list of all the available (completed) subassembly orders for that specific sale order will appear. Select the subassembly order that was used for this specific SF number.
5. After you submit the form, the SF number subassembly confirmation will be done and the **selected subassemblies will be linked to the SF number**.

<iframe src="https://drive.google.com/file/d/17wkQzEF9pMk86YJCOneoKYI4CyZB-3SD/preview" width="711" height="400" allow="autoplay; fullscreen" allowfullscreen="true" frameborder="0"></iframe>

---

## 6. Accessing Logs and Dashboards

### Confirmation Logs
1. Navigate to the **stages section** of a specific Subassembly order.
2. Click the **‘View Logs’** button on the right side of the stage.
3. Logs are sorted from most recent to oldest.
4. Click **‘View Details’** to see any further information entered by the user during that action.

### Subassembly Linkage Logs
1. Navigate to the **stages section** of a specific work order.
2. Click the **‘View Logs’** button on the right side of the stage.
3. Logs are sorted from most recent to oldest.
4. Click **‘View Details’** to see any further information entered by the user during that action.
5. You will see the selected subassembly orders selected while completing the subassembly confirmation for the SF number. Click on the subassembly order and you will be taken to the subassembly confirmation logs. 
6. **This way you can check all the subassembly related details that were used for assembling the particular FG**. 

<iframe src="https://drive.google.com/file/d/1l_-_v4ZdusvngTrEE1Yb7ZdolkjScfBG/preview" width="711" height="400" allow="autoplay; fullscreen" allowfullscreen="true" frameborder="0"></iframe>

### Sub Assembly Report
1. Click the **‘View PPC Dashboard’** button on the landing page.
2. Select the **Sub Assembly** tab from the top right corner. 
    - This report shows the produced subassemblies against the sale orders they were created against.

<iframe src="https://drive.google.com/file/d/1SnNpuQ4FYf9gc8XvYCKvXIeqPC2bBBTu/preview" width="711" height="400" allow="autoplay; fullscreen" allowfullscreen="true" frameborder="0"></iframe>

---

## 7. Complete Demo

The following demo takes the user through different flows to explain how the tracking feature can be used to link the subassemblies to the SF numbers.

<iframe src="https://drive.google.com/file/d/1ZhgFf4tBlh6U_BI5yYLWak22bUGDI-3-/preview" width="711" height="400" allow="autoplay; fullscreen" allowfullscreen="true" frameborder="0"></iframe>