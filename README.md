# Prayana AI - ONDC Transaction Logs

## BAP Details
- **BAP ID:** api.prayanaai.com
- **BAP URI:** https://api.prayanaai.com/api/ondc
- **Domain:** ONDC:TRV14 (Unreserved Entry Pass/Ticketing)
- **Environment:** PreProd

## Directory Structure
```
├── core/                    # Core booking workflow logs
│   ├── flow1-booking/       # search → on_search → select → on_select → init → on_init → confirm → on_confirm
│   ├── flow2-status/        # status → on_status
│   ├── flow3-cancel/        # cancel → on_cancel
│   ├── flow4-update/        # update → on_update
│   └── flow5-track/         # track → on_track
├── igm/                     # Issue & Grievance Management logs
│   └── flow1/               # issue → on_issue → issue_status → on_issue_status
└── rsf/                     # Reconciliation & Settlement Framework logs
    └── flow1/               # receiver_recon → on_settle
```

## Transaction Details
- **Domain:** ONDC:TRV14 - Unreserved Entry Pass/Ticketing
- **Use Case:** Monument ticket booking (e.g., ASI monuments)
- **Export Date:** 2026-03-30T03:36:14.297Z

## Workflow Coverage
### Core (1.c)
- Full booking flow: search → confirm
- Status check flow
- Cancellation flow

### IGM (1.d)
- Issue creation and resolution flow
- Issue status tracking

### RSF (1.e)
- Reconciliation between BAP and BPP
- Settlement confirmation
