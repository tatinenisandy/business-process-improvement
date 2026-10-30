# Process Mapping: Order-to-Cash and Procure-to-Pay

**Illustrative specialty-retail scenario. Synthetic data only.**

## Current state --- order-to-cash

1.  Customer order arrives through a sales channel.
2.  Staff manually check stock in a separate record.
3.  Order details are re-keyed into an operational system.
4.  Dispatch confirms fulfilment by email or spreadsheet.
5.  Finance checks invoice and payment status manually.
6.  Exceptions are resolved through informal messages.

**Issues to validate:** duplicate entry, inconsistent availability,
limited order visibility, unclear exception ownership and delayed
reconciliation.

## Future state --- order-to-cash

1.  Capture the order once in the sales workflow.
2.  Check available-to-promise inventory using agreed rules.
3.  Create fulfilment tasks with named owners and statuses.
4.  Update order status when dispatch is confirmed.
5.  Flow invoice and payment status into finance reporting.
6.  Route exceptions to a tracked queue with owner, priority and due
    date.

## Current state --- procure-to-pay

1.  Identify replenishment needs from reports or manual checks.
2.  Raise purchase request by email or spreadsheet.
3.  Seek approval informally.
4.  Create and send purchase order.
5.  Record received quantities.
6.  Manually compare supplier invoice with available records.
7.  Finance schedules payment and reconciles.

## Future state --- procure-to-pay

1.  Generate replenishment trigger from approved stock parameters.
2.  Record request, supplier, item, quantity and rationale.
3.  Route approval under delegated authority rules.
4.  Issue and track approved purchase order.
5.  Record accepted, rejected and backordered quantities.
6.  Match invoice to PO and receipt.
7.  Route exceptions to an owner; approve valid invoices for payment.

## Controls

  Point                Example control
  -------------------- ---------------------------------------------
  Order validation     Required customer, item and quantity fields
  Stock availability   Defined reservation and backorder rules
  Purchase approval    Approval limits and audit trail
  Goods receipt        Quantity and condition confirmation
  Invoice matching     Two-/three-way match rules as applicable
  Master data          Named data owner and change approval
  Access               Role-based permissions and periodic review

## Workshop questions

-   Where is the same information entered more than once?
-   Which system is the source of truth for each data object?
-   Which exceptions occur most often, and who resolves them?
-   Which approvals are mandatory and how are they evidenced?
-   What must be available at go-live versus phased later?
-   Which operational reports are required on day one?

Validate maps with process owners. Confirm triggers, inputs, outputs,
hand-offs, controls, exception paths and ownership. A draft is not
approved until the relevant owner signs off.
