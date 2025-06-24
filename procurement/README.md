# Schema for Procurement System

## Complete Procurement Workflow

ระบบจัดซื้อจัดจ้างครบวงจร ตั้งแต่การขอซื้อจนถึงการรับสินค้า

### Workflow:
1. **Purchase Requisition (PR)** - ใบขอซื้อ
2. **Request for Quotation (RFQ)** - ใบขอใบเสนอราคา
3. **Quotation** - ใบเสนอราคาจากผู้ขาย
4. **Purchase Order (PO)** - ใบสั่งซื้อ
5. **Goods Receipt (GR)** - ใบรับสินค้า

### Collections:

#### Master Data:
1. **suppliers** - ข้อมูลผู้จัดจำหน่าย/ผู้ขาย

#### Purchase Requisition:
2. **purchase_requisitions** - ใบขอซื้อ (PR)
3. **purchase_requisition_items** - รายการสินค้าในใบขอซื้อ

#### Request for Quotation:
4. **request_for_quotations** - ใบขอใบเสนอราคา (RFQ)
5. **rfq_suppliers** - ผู้ขายที่ส่ง RFQ ให้
6. **rfq_items** - รายการสินค้าใน RFQ

#### Quotation:
7. **quotations** - ใบเสนอราคา
8. **quotation_items** - รายการสินค้าในใบเสนอราคา

#### Purchase Order:
9. **purchase_orders** - ใบสั่งซื้อ (PO)
10. **purchase_order_items** - รายการสินค้าในใบสั่งซื้อ

#### Goods Receipt:
11. **goods_receipts** - ใบรับสินค้า (GR)
12. **goods_receipt_items** - รายการสินค้าในใบรับสินค้า

### Key Features:
- ระบบอนุมัติหลายระดับ
- เปรียบเทียบใบเสนอราคาจากหลายผู้ขาย
- ติดตามสถานะการสั่งซื้อ
- จัดการข้อมูลผู้ขาย
- ควบคุมปริมาณการรับสินค้า
- รายงานและการติดตาม 