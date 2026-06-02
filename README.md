# ◤◢ ARES-LAB-FRASDORF // NODE-ALPHA: BASE HARDWARE PROTOCOL ◣◥
================================================================================
 [PROPERTY_OF: ARES_LAB_FRASDORF]
 [GENESIS_ID:  ARES-NODE-ALPHA-2026]
 [SECURITY_CLASS: SOVEREIGN_LOCAL_CORE]
 [DIGITAL_WATERMARK: VERIFIED_BY_ARES_CORE_INFRASTRUCTURE_2026]
================================================================================

## 1. HARDWARE CORE & MEMORY STATUS
* **CPU:** AMD Ryzen 9 9950X ──> [STATUS: ACTIVE]
  * *Notes:* Erfolgreich im Sockel arretiert. Kühlung via KryoSheet (keine Paste).
* **GPU:** NVIDIA RTX 4000 Ada SFF 20GB VRAM ──> [STATUS: INSTALLED]
  * *Notes:* Physisch fixiert im primären Slot 1 für lokale KI-Vektorisierung.
* **MB:** ASUS ROG Strix X870E Gaming WiFi ──> [STATUS: ACTIVE]
  * *Notes:* Kern-Infrastruktur für 4-Bank-Betrieb und Peripherie-Management.
* **RAM Workstation:** 32GB Crucial/Micron DDR5 ──> [STATUS: LOCKED]
  * *Notes:* Bestückt in Slots A2 & B2. Initiales RAM-Training im BIOS erfolgreich abgeschlossen (Werksprofil: 5600 MHz稳定).
* **SSD:** Crucial T710 Gen5 2TB (`CT2000T7105SD8`) ──> [STATUS: INSTALLED]
  * *Notes:* Montiert im Slot M.2_1 (Direkte CPU-Anbindung).
* **COOLING:** Corsair iCUE LINK RX360 AIO ──> [STATUS: OPERATIONAL]
  * *Notes:* Display läuft, Lüfterbänke synchronisiert. Idle-Temperaturen stabil bei hervorragenden 34°C - 40°C.

## 2. MAINBOARD TOPOLOGY & PCIe LANE ROUTING LOGIC
* **Slot 1 (PCIe 5.0 x16):** Exklusiv reserviert für RTX 4000 Ada SFF (Volle x16 Bandbreite für lokale LLMs).
* **Slot 2 (PCIe 4.0 x4):** Fest verplant für dedizierte LAN-Karte (Anbindung an das Kellerbiest über den Chipsatz). Verhindert jegliche Drosselung der Grafikkarte.
* **Slot 3 (PCIe 4.0 x4):** Frei für zukünftige Erweiterungen (z.B. PCIe-USB-Erweiterungskarte).
* **⚠️ CRITICAL SECURITY RULE:** Der Slot **M.2_2** MUSS permanent frei bleiben! Sobald dort eine SSD eingesetzt wird, halbiert das Board automatisch die Lanes der GPU auf x8. Zusätzlicher Speicherplatz darf ausschließlich über die Slots M.2_3 oder M.2_4 nachgerüstet werden.

## 3. POWER, DATA & USB INTERFACE ROUTING
* **Corsair iCUE LINK System-Hub:** Stromversorgung erfolgt kombiniert über die dedizierte PCIe-Kabelpeitsche direkt vom vollmodularen Netzteil.
* **USB-Header-Engpass:** Erfolgreich gelöst via Corsair USB-Y-Splitter. Die AIO-Steuerung und die digitale Netzteil-Schnittstelle (HX1000i Typ-C Datenleitung) teilen sich einen einzigen physischen 9-Pin-Mainboard-Header. Verkabelung im Corsair 6500X Aquarium bleibt absolut "clean".
* **Interim-PSU:** Corsair HX1000i versorgt den Testbetrieb fehlerfrei.
* **Target-PSU:** Corsair HX1500i Shift [INBOUND / EXPECTED 2026-06-02]. Nach Eintreffen wird ein aktiver, SATA-stromversorgter interner USB-Hub im Heck integriert.

## 4. SYSTEM ARCHITECTURE & OS PIPELINE
* **Primary OS:** Windows 11 Pro (Legale Lifetime-OEM-Vollversion ohne Abo-Zwang). Zwingend erforderlich für native iCUE LINK/Display-Infrastruktur und optimalen Thread-Scheduler des 9950X.
* **Security Layer:** Keine Drittanbieter-Antivirensoftware. Windows Defender fungiert als schlanker, kernelnaher Schutz.
* **Open-Source-Deployment:** Grundausstattung (Firefox, LibreOffice, 7-Zip, VLC, Notepad++) wird automatisiert via `winget` auf die T710 geschrieben.
* **Secondary OS:** Kubuntu Linux wird im Dual-Boot verankert (dedizierter Speicherbereich auf der T710 bleibt unpartitioniert frei) für autarke SDR-Frequenzüberwachung.

================================================================================
 [DIGITAL_SIGNATURE: SHA256_ARES_LAB_VERIFIED]
 [STATUS: INFRASTRUCTURE_READY // WAITING FOR PSU_TARGET_UPGRADE]
================================================================================
