# ARES-Infrastructure-Core
ARES-Infrastructure-Core: Zentrales Repository für technisches Hardware-Management, SDR-Datenanalyse und KI-Projekt-Konfiguration. Fokus auf stabile Infrastruktur (Server-Cluster, HP-Scanner-Nodes), automatisierte Dokumentation und Optimierung von System-Leistungsparametern für den 24/7 Betrieb.
<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/6803ed74-f375-48cf-b2dc-454bec70a8a7" />
<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/19a3b3fd-8a46-4b8e-8158-3ab70d04e29c" />
# LAB-LOGBOOK: PHASE_01_PREPARATION
[SYSTEM_STATUS: NIGHT_SHIFT_ROSENHEIM // TIMESTAMP: 2026-05-30_21:30]

## 1. HARDWARE_INVENTORY_STATUS
- CPU: AMD Ryzen 9 9950X (Box-Version) -> unexpected early delivery confirmed via [IMG-20260530-WA0008.jpg]
- GPU: NVIDIA RTX 4000 Ada SFF 20GB VRAM -> procured in Jan for 1250€ (current market value 2050€)
- MB: ASUS X870 Max Gaming
- RAM: Samsung DDR5 (Vollbestückung / 4 Bänke vorbereitet)
- SSD: Crucial T710 Gen5 8TB Total Pool
- COOLING: Corsair iCUE LINK RX360 AIO + LX-Fan-Chains
- PSU: Corsair HX1000i (Interim Saftspender) // Shift HX1500i ordered for 274€

## 2. DEPLOYMENT_STRATEGY_SUNDAY (2026-05-31)
- FOCUS: Mechanical assembly & "Trockenschwimmen" inside Corsair 6500X.
- STEP_01: Motherboard installation, mount Crucial T710 under heatspreader.
- STEP_02: RAM training preparation (Insert 2 modules in slots A2 & B2 for initial boot stability).
- STEP_03: Cable routing for iCUE LINK ecosystem, space & weight validation.
- STEP_04: CPU unboxing & inspection (Verify Alexa's "9950X3D" claim vs. real 9950X compute weapon).
- STEP_05: Socket placement, Grizzly-Pad application, AIO mounting.

## 3. FIRMWARE_UPDATE_STRATEGY_MONDAY
- TARGET_VERSION: BIOS 1670 (Beta, AGESA memory profile support for 4-bank stability).
- METHOD: EZ Flash via BIOS-GUI (Post-CPU installation with 2 RAM sticks, monitor active).
- MEDIA: 8GB USB stick, native FAT32 format, file manually renamed to A5669.CAP via BIOSRenamer.

## 4. NEXT_MILESTONE_LOCAL_AI
- TARGET: Complete sovereign offline infrastructure on Ada SFF + 9950X.
- ARCHITECTURE: Local VectorDB (Qdrant/Milvus) on Gen5 SSD to bypass cloud context limits entirely.

