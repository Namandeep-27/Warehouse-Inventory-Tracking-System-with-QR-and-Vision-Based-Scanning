# Warehouse-Inventory-Tracking-System-with-QR-and-Vision-Based-Scanning
AI-assisted warehouse inventory tracking system using QR scanning and vision-based detection to automate box movement, maintain real-time stock visibility, and reduce manual logging. Includes workflow validation, placement logic, and operational dashboards for smarter warehouse operations.

Entry and exit are detected through CCTV scanning, automatically registering boxes without manual logging. The system maintains real time inventory, movement history, and a dashboard showing stock and activity. It suggests shelf locations based on product activity so staff can place boxes where recommended. If another shelf is used, staff can scan the shelf and box with an iPad to record placement. The system prevents duplicate scans and is designed to evolve into a CCTV-driven workflow.

Architecture Overview

The platform is designed as a modular full-stack system that combines operational workflow intelligence with computer vision-assisted data capture.
	•	Frontend: React-based operator dashboard for inventory actions and activity monitoring
	•	Backend: Node.js API layer managing inventory state, movement validation, and workflow orchestration
	•	Database: Structured data models for products, boxes, locations, and activity logs
	•	Vision Layer: Computer vision pipeline for QR detection and scan validation
	•	Workflow Engine: Rule-based logic controlling inventory lifecycle transitions

⸻

Tech Stack
	•	Frontend: React, Vite, Tailwind CSS
	•	Backend: Node.js, TypeScript, Express
	•	Database: SQL-based structured storage
	•	Computer Vision: Python, OpenCV, Object Detection workflows
	•	System Design: Modular API architecture with configurable operational rules

⸻
<img width="2932" height="1596" alt="image" src="https://github.com/user-attachments/assets/94a5386b-7b40-442a-91ef-806ebab79773" />
Warehouse operations dashboard with real-time stats and quick actions for receiving, moving, and shipping inventory.
<img width="2570" height="1568" alt="image" src="https://github.com/user-attachments/assets/fe2f5bd8-bb46-4649-8669-8f46b8388e0e" />
Home page (below): put-away queue for boxes awaiting shelf placement with a live activity feed of received, moved, and shipped events.
<img width="2594" height="1588" alt="image" src="https://github.com/user-attachments/assets/97309e4b-8ce5-4a2d-bd98-346d8cdf4f24" />
Product catalog where admins define items (brand, product, size) before generating box labels and tracking inventory.
<img width="2198" height="1584" alt="image" src="https://github.com/user-attachments/assets/3902e55a-2737-47f2-bda7-bf89c266f138" />
Generate QR labels for warehouse boxes by selecting a product and lot code. Each box receives a unique ID for tracking.
<img width="2010" height="1282" alt="image" src="https://github.com/user-attachments/assets/8f2dab8c-ea34-45e8-bff2-5df312858071" />
Generated QR box label with a unique box ID that can be printed and attached to physical boxes for camera-based tracking.
<img width="2040" height="1526" alt="image" src="https://github.com/user-attachments/assets/6b2ae332-486d-40ec-8397-806afbb71a80" />
Entry CCTV scans the box QR code and automatically registers the product, lot code, and box ID as received in inventory.
<img width="2566" height="656" alt="image" src="https://github.com/user-attachments/assets/2f22b567-9157-4a63-832a-bdbcf775eeb3" />
Locations page where warehouse shelf positions are defined and QR codes are generated for tracking box placement.
<img width="814" height="928" alt="image" src="https://github.com/user-attachments/assets/d5b6f7a0-c406-441f-949c-0991f76b33bc" />
The system suggests shelf locations for boxes. Staff can scan with iPads if needed, with future support for fully automated CCTV tracking.
<img width="2072" height="1516" alt="image" src="https://github.com/user-attachments/assets/252ebc6f-ae11-41fb-8316-8978988d64fd" />
Box relocated by scanning the shelf QR first, then the box. System updates the exact warehouse location instantly.
<img width="2532" height="1594" alt="image" src="https://github.com/user-attachments/assets/55bd99a0-ab46-4058-a1bb-a36b6744c4c5" />
Inventory page shows all boxes in stock with filters for product, location, and status to quickly find items in the warehouse.
<img width="2510" height="1458" alt="image" src="https://github.com/user-attachments/assets/d0e958c7-2be1-4ccb-b887-fb469ce47059" />
The inventory page shows all boxes with filters for product, status, location, and date, helping staff quickly find items in the warehouse.
