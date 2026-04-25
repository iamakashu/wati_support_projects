### 1. Project Summary

This project involves the implementation of an end-to-end RFID (Radio Frequency Identification) tracking system within the central distribution center to replace manual barcode scanning. This initiative will provide real-time inventory visibility, drastically reduce human error during the picking and packing process, and ensure 99.9% order accuracy for e-commerce fulfillment.

### 2. Tools & Technologies

- **Hardware:** Zebra FX9600 Fixed RFID Readers and handheld scanners.
- **Tags:** EPC Gen 2 Passive RFID adhesive tags.
- **Software:** Fishbowl Inventory Management System integration.
- **Database:** SQL Server for local data caching and synchronization.
- **Middleware:** Custom Python-based API for ERP-to-Hardware communication.

### 3. Scope

**In-Scope:**

- Installation of RFID portals at Receiving and Outbound Shipping docks.
- Tagging of all current SKUs (approx. 500 unique items) and incoming stock.
- API integration between RFID hardware and the existing e-commerce storefront.
- Staff training for 15 warehouse floor employees.

**Out-Of-Scope:**

- Automation of physical movement (e.g., robotics or conveyor belts).
- Integration with third-party logistics (3PL) partner systems.
- Re-design of the physical warehouse layout or shelving.

### 4. Plan

- **Month 1:** Hardware procurement, site survey, and network infrastructure upgrades.
- **Month 2:** Tagging phase and API development for ERP synchronization.
- **Month 3:** System stress testing and staff training workshops.
- **Q3 Start:** Go-live and decommissioning of legacy barcode handhelds.

### 5. Measurable KPIs

| Metric / KPI              | Baseline (Current) | Target (Post-Project) | Measurement Method        |
| ------------------------- | ------------------ | --------------------- | ------------------------- |
| Inventory Audit Time      | 16 Man-Hours       | 45 Minutes            | Time-motion study         |
| Order Picking Accuracy    | 94.2%              | 99.9%                 | Returns/Mis-shipment Logs |
| Stock Shrinkage           | 2.5% Annual        | < 0.5% Annual         | Quarterly Cycle Counts    |
| Daily Processing Capacity | 400 Orders         | 750 Orders            | ERP Fulfillment Reports   |