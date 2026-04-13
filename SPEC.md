# Electric Rental & Repairing Shop - Web Application Specification

## Project Overview
- **Project Name**: Electric Shop Manager
- **Type**: Single Page Web Application
- **Core Functionality**: Complete business management system for electric rental & repairing shop
- **Target Users**: Shop owners, billing staff

## UI/UX Specification

### Layout Structure
- **Header**: Company logo/name, navigation menu
- **Sidebar**: Navigation menu with icons
- **Main Content Area**: Dynamic content based on selected module
- **Footer**: Copyright info

### Responsive Breakpoints
- Desktop: > 1024px
- Tablet: 768px - 1024px
- Mobile: < 768px

### Visual Design
- **Color Palette**:
  - Primary: #1a1a2e (Dark Navy)
  - Secondary: #16213e (Deep Blue)
  - Accent: #e94560 (Red/Pink)
  - Success: #00d9a5 (Green)
  - Warning: #ffc107 (Amber)
  - Background: #0f0f1a (Dark)
  - Card Background: #1f1f35 (Dark Purple)
  - Text Primary: #ffffff
  - Text Secondary: #a0a0b0
  
- **Typography**:
  - Font Family: 'Segoe UI', system-ui, sans-serif
  - Headings: Bold, 1.5rem - 2rem
  - Body: Regular, 0.9rem - 1rem

- **Spacing**: 8px base unit (0.5rem, 1rem, 1.5rem, 2rem)

- **Visual Effects**:
  - Card shadows: 0 4px 20px rgba(0,0,0,0.3)
  - Hover transitions: 0.3s ease
  - Border radius: 8px-12px

### Components
- Navigation tabs with active states
- Form inputs with floating labels
- Data tables with sorting
- Modal dialogs for forms
- Date pickers for report filtering
- Print-friendly invoice layout

## Functionality Specification

### 1. Company Profile
- Company name
- Owner name
- Address
- Phone number
- Email
- GST Number
- Logo upload (optional)

### 2. Customer Management
- Customer name
- Customer type (Retail/Wholesale)
- Phone number
- Email
- GST Number (optional)
- Address
- Created date

### 3. Product/Item Management
- Item name
- Item code/SKU
- Category (Rental/Repair/Parts)
- HSN Code
- GST Rate
- Purchase price
- Rental price
- Repair charge
- Current stock quantity
- Minimum stock alert

### 4. Purchase Management
- Purchase date
- Supplier name
- Invoice number
- Item selection
- Quantity
- Rate
- GST amount
- Total amount
- Payment status (Paid/Unpaid)

### 5. Sales/Invoice Generation
- Invoice number (auto-generated)
- Invoice date
- Customer selection
- Item selection with quantity
- Rate, GST calculation
- Subtotal, CGST, SGST, Total
- Payment mode (Cash/Card/Online)
- Print invoice option

### 6. Stock Maintenance
- Current stock view
- Add/Remove stock
- Stock adjustment
- Low stock alerts

### 7. Reports
- **Stock Report**: Current inventory status
- **Purchase Report**: Date to date purchase summary
- **Sales Report**: Date to date sales summary
- Date range picker for all reports
- Print/Export option

### 8. Dashboard
- Today's sales
- Monthly sales
- Total customers
- Low stock items count
- Recent transactions

## Data Storage
- LocalStorage for data persistence
- JSON format for all records

## Acceptance Criteria
1. All navigation links work correctly
2. Forms save data to localStorage
3. Invoice generates with proper calculations
4. Reports filter by date range correctly
5. Stock updates automatically on purchase/sale
6. Print functionality works for invoices
7. Data persists across browser sessions
8. Responsive design works on all devices
