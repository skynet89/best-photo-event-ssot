# Best Photo Event (BPE)

Best Photo Event è una piattaforma commerciale multi-tenant per la vendita di fotografie durante eventi, con architettura Edge + Cloud.

## Architettura

- 🖥 Edge Server (Linux on-prem)
- 📱 Kiosk Android (touchscreen per clienti)
- ☁ Cloud Control Plane (SaaS)
- 🔐 Licenze firmate Ed25519
- 🖨 Hotfolder printing (default)
- 📊 Dashboard vendite e royalties

---

## Modalità Operativa

### Edge (offline-first)
- Upload foto da postazione fotografo
- Generazione automatica watermark
- Navigazione foto su monitor touch
- Creazione ordine + QR ticket
- Stampa solo dopo pagamento
- Sync periodico verso Cloud

### Cloud (saas-photoapp.digitalsupport.eu)
- Gestione tenant
- Gestione edge devices
- Emissione licenze
- Monitoraggio check-in
- Report vendite
- Royalty management

---

## SSOT - Single Source of Truth

Questa repository contiene i contratti ufficiali v1:
