# Kiosk Pairing v1 (No camera assumption)

Kiosk pairing must support:
1) LAN discovery: GET /.well-known/bpe-edge on candidate edge hosts
2) Manual code pairing:
   - Staff creates code: POST /api/setup/pair/request (auth staff)
   - Kiosk confirms: POST /api/pair/confirm with code + kiosk_info
   - Codes are single-use, expire within 5 minutes
3) Enforce license max_kiosks at pairing time
