# UI/UX Wireframes and Design Specifications

## Design System

### Color Palette
```css
:root {
  /* Primary Colors */
  --primary-50: #f0f9ff;
  --primary-100: #e0f2fe;
  --primary-500: #0ea5e9;
  --primary-600: #0284c7;
  --primary-700: #0369a1;
  --primary-900: #0c4a6e;

  /* Secondary Colors */
  --secondary-50: #f8fafc;
  --secondary-100: #f1f5f9;
  --secondary-500: #64748b;
  --secondary-600: #475569;
  --secondary-700: #334155;
  --secondary-900: #0f172a;

  /* Status Colors */
  --success-500: #10b981;
  --warning-500: #f59e0b;
  --error-500: #ef4444;
  --info-500: #3b82f6;

  /* Neutral Colors */
  --gray-50: #f9fafb;
  --gray-100: #f3f4f6;
  --gray-200: #e5e7eb;
  --gray-300: #d1d5db;
  --gray-400: #9ca3af;
  --gray-500: #6b7280;
  --gray-600: #4b5563;
  --gray-700: #374151;
  --gray-800: #1f2937;
  --gray-900: #111827;
}
```

### Typography
```css
/* Font Families */
--font-primary: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', monospace;

/* Font Sizes */
--text-xs: 0.75rem;    /* 12px */
--text-sm: 0.875rem;   /* 14px */
--text-base: 1rem;     /* 16px */
--text-lg: 1.125rem;   /* 18px */
--text-xl: 1.25rem;    /* 20px */
--text-2xl: 1.5rem;    /* 24px */
--text-3xl: 1.875rem;  /* 30px */
--text-4xl: 2.25rem;   /* 36px */

/* Font Weights */
--font-normal: 400;
--font-medium: 500;
--font-semibold: 600;
--font-bold: 700;
```

### Spacing System
```css
/* 8px base unit */
--space-1: 0.25rem;   /* 4px */
--space-2: 0.5rem;    /* 8px */
--space-3: 0.75rem;   /* 12px */
--space-4: 1rem;      /* 16px */
--space-5: 1.25rem;   /* 20px */
--space-6: 1.5rem;    /* 24px */
--space-8: 2rem;      /* 32px */
--space-10: 2.5rem;   /* 40px */
--space-12: 3rem;     /* 48px */
--space-16: 4rem;     /* 64px */
--space-20: 5rem;     /* 80px */
```

## Admin Dashboard Wireframes

### 1. Admin Login Page
```
┌─────────────────────────────────────────────────────────────┐
│                        TrackAS                              │
│                    Admin Portal                             │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│    ┌─────────────────────────────────────────────────┐     │
│    │                                                 │     │
│    │              Admin Login                        │     │
│    │                                                 │     │
│    │  Email:    [________________________]          │     │
│    │                                                 │     │
│    │  Password: [________________________]          │     │
│    │                                                 │     │
│    │            [  Login  ]                         │     │
│    │                                                 │     │
│    │            Forgot Password?                     │     │
│    │                                                 │     │
│    └─────────────────────────────────────────────────┘     │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### 2. Admin Dashboard Overview
```
┌─────────────────────────────────────────────────────────────┐
│ TrackAS Admin │ Dashboard │ Approvals │ Settings │ Logout   │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│ ┌─────────────┐ ┌─────────────┐ ┌─────────────┐ ┌─────────┐ │
│ │   Pending   │ │   Active    │ │   Total     │ │Revenue  │ │
│ │ Approvals   │ │ Shipments   │ │ Companies   │ │This Month│ │
│ │     15      │ │    1,234    │ │     456     │ │₹2.5L    │ │
│ └─────────────┘ └─────────────┘ └─────────────┘ └─────────┘ │
│                                                             │
│ ┌─────────────────────────────────────────────────────────┐ │
│ │                Recent Activities                        │ │
│ │ • New company registration: ABC Logistics               │ │
│ │ • Driver verification completed: John Doe               │ │
│ │ • Vehicle approved: MH01AB1234                         │ │
│ │ • Support ticket resolved: #TKT001                     │ │
│ └─────────────────────────────────────────────────────────┘ │
│                                                             │
│ ┌─────────────────────────────────────────────────────────┐ │
│ │                 Quick Actions                           │ │
│ │ [Review Pending Approvals] [Commission Settings]       │ │
│ │ [Generate Reports]         [System Settings]           │ │
│ └─────────────────────────────────────────────────────────┘ │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### 3. Approval Workflow Page
```
┌─────────────────────────────────────────────────────────────┐
│ TrackAS Admin │ Dashboard │ Approvals │ Settings │ Logout   │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│ Pending Approvals                                           │
│                                                             │
│ ┌─────────────┐ ┌─────────────┐ ┌─────────────┐            │
│ │ Companies   │ │  Drivers    │ │  Vehicles   │            │
│ │    (8)      │ │    (12)     │ │    (5)      │            │
│ └─────────────┘ └─────────────┘ └─────────────┘            │
│                                                             │
│ ┌─────────────────────────────────────────────────────────┐ │
│ │ Company: ABC Logistics                    [View Details]│ │
│ │ Email: abc@logistics.com                               │ │
│ │ Registration: 2024-01-15                               │ │
│ │ Documents: ✓ GST ✓ PAN ✓ Bank Details                 │ │
│ │ [Approve] [Reject] [Request More Info]                 │ │
│ ├─────────────────────────────────────────────────────────┤ │
│ │ Driver: John Doe                          [View Details]│ │
│ │ License: DL123456789                                   │ │
│ │ Phone: +919876543210                                   │ │
│ │ Documents: ✓ License ✓ Aadhar ✓ Bank Details          │ │
│ │ [Approve] [Reject] [Request More Info]                 │ │
│ └─────────────────────────────────────────────────────────┘ │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### 4. Commission Settings Page
```
┌─────────────────────────────────────────────────────────────┐
│ TrackAS Admin │ Dashboard │ Approvals │ Settings │ Logout   │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│ Commission Settings                                         │
│                                                             │
│ ┌─────────────────────────────────────────────────────────┐ │
│ │ Global Settings                                         │ │
│ │                                                         │ │
│ │ Default Commission Rate: [5.00] %                       │ │
│ │ Maximum Commission Rate: [10.00] %                      │ │
│ │ Minimum Commission Rate: [2.00] %                       │ │
│ │                                                         │ │
│ │ Commission Collection:                                  │ │
│ │ ○ Before Shipment (Prepaid)                            │ │
│ │ ● After Delivery (Postpaid)                            │ │
│ │                                                         │ │
│ │ Auto-deduction from payments: ☑ Enabled                │ │
│ │                                                         │ │
│ │ [Save Settings]                                         │ │
│ └─────────────────────────────────────────────────────────┘ │
│                                                             │
│ ┌─────────────────────────────────────────────────────────┐ │
│ │ Company-specific Rates                                  │ │
│ │                                                         │ │
│ │ ABC Logistics        5.0%    [Edit]                     │ │
│ │ XYZ Transport        4.5%    [Edit]                     │ │
│ │ FastMove Logistics   5.5%    [Edit]                     │ │
│ │                                                         │ │
│ │ [Add Custom Rate]                                       │ │
│ └─────────────────────────────────────────────────────────┘ │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

## Company Dashboard Wireframes

### 1. Company Login Page
```
┌─────────────────────────────────────────────────────────────┐
│                        TrackAS                              │
│                  Logistics Portal                           │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│    ┌─────────────────────────────────────────────────┐     │
│    │                                                 │     │
│    │            Company Login                        │     │
│    │                                                 │     │
│    │  Email:    [________________________]          │     │
│    │                                                 │     │
│    │  Password: [________________________]          │     │
│    │                                                 │     │
│    │            [  Login  ]                         │     │
│    │                                                 │     │
│    │  Don't have an account? Register               │     │
│    │            Forgot Password?                     │     │
│    │                                                 │     │
│    └─────────────────────────────────────────────────┘     │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### 2. Company Dashboard
```
┌─────────────────────────────────────────────────────────────┐
│ TrackAS │ Dashboard │ Shipments │ Drivers │ Payments │ Profile│
├─────────────────────────────────────────────────────────────┤
│                                                             │
│ Welcome back, ABC Logistics                                 │
│                                                             │
│ ┌─────────────┐ ┌─────────────┐ ┌─────────────┐ ┌─────────┐ │
│ │   Active    │ │ Completed   │ │   Pending   │ │Revenue  │ │
│ │ Shipments   │ │ This Month  │ │  Payments   │ │This Month│ │
│ │     23      │ │    156      │ │   ₹45,000   │ │₹2.8L    │ │
│ └─────────────┘ └─────────────┘ └─────────────┘ └─────────┘ │
│                                                             │
│ ┌─────────────────────────────────────────────────────────┐ │
│ │ [+ Create New Shipment]                                 │ │
│ └─────────────────────────────────────────────────────────┘ │
│                                                             │
│ ┌─────────────────────────────────────────────────────────┐ │
│ │                Recent Shipments                         │ │
│ │ ┌─────────────────────────────────────────────────────┐ │ │
│ │ │ TRK001 │ Electronics │ Mumbai→Pune │ In Transit    │ │ │
│ │ │ TRK002 │ Furniture   │ Delhi→Goa   │ Delivered     │ │ │
│ │ │ TRK003 │ Textiles    │ Chennai→Kochi│ Picked Up    │ │ │
│ │ └─────────────────────────────────────────────────────┘ │ │
│ │ [View All Shipments]                                    │ │
│ └─────────────────────────────────────────────────────────┘ │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### 3. Create Shipment Page
```
┌─────────────────────────────────────────────────────────────┐
│ TrackAS │ Dashboard │ Shipments │ Drivers │ Payments │ Profile│
├─────────────────────────────────────────────────────────────┤
│                                                             │
│ Create New Shipment                                         │
│                                                             │
│ ┌─────────────────────────────────────────────────────────┐ │
│ │ Shipment Details                                        │ │
│ │                                                         │ │
│ │ Title: [_________________________________]              │ │
│ │ Description: [________________________]                 │ │
│ │                                                         │ │
│ │ Priority: ○ Normal ○ High ○ Urgent                      │ │
│ │                                                         │ │
│ │ Goods Type: [Electronics ▼]                            │ │
│ │ Goods Value: ₹[__________]                              │ │
│ │                                                         │ │
│ │ Weight: [____] kg  Dimensions: [__]×[__]×[__] cm       │ │
│ │                                                         │ │
│ │ Special Instructions:                                   │ │
│ │ [_____________________________________________]         │ │
│ └─────────────────────────────────────────────────────────┘ │
│                                                             │
│ ┌─────────────────────────────────────────────────────────┐ │
│ │ Pickup Details                                          │ │
│ │                                                         │ │
│ │ Address: [_________________________________]            │ │
│ │ Contact: [________________] Phone: [__________]         │ │
│ │ Pickup Date: [__________] Time: [________]              │ │
│ │                                                         │ │
│ │ [📍 Select on Map]                                      │ │
│ └─────────────────────────────────────────────────────────┘ │
│                                                             │
│ ┌─────────────────────────────────────────────────────────┐ │
│ │ Delivery Details                                        │ │
│ │                                                         │ │
│ │ Address: [_________________________________]            │ │
│ │ Contact: [________________] Phone: [__________]         │ │
│ │ Expected Date: [__________] Time: [________]            │ │
│ │                                                         │ │
│ │ [📍 Select on Map]                                      │ │
│ └─────────────────────────────────────────────────────────┘ │
│                                                             │
│ ┌─────────────────────────────────────────────────────────┐ │
│ │ Pricing                                                 │ │
│ │                                                         │ │
│ │ Shipment Cost: ₹[_______]                               │ │
│ │ Commission (5%): ₹[_____] (Auto-calculated)            │ │
│ │ Net Payout: ₹[_______]                                  │ │
│ │                                                         │ │
│ │ Payment Method: ○ Online ○ Cash on Delivery             │ │
│ └─────────────────────────────────────────────────────────┘ │
│                                                             │
│ [Cancel] [Save as Draft] [Create Shipment]                 │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### 4. Shipment Tracking Page
```
┌─────────────────────────────────────────────────────────────┐
│ TrackAS │ Dashboard │ Shipments │ Drivers │ Payments │ Profile│
├─────────────────────────────────────────────────────────────┤
│                                                             │
│ Shipment Details - TRK123456789                            │
│                                                             │
│ ┌─────────────────────────────────────────────────────────┐ │
│ │ Status: In Transit        ETA: 2 hours 30 minutes      │ │
│ │ Driver: John Doe          Vehicle: MH01AB1234          │ │
│ │ Phone: +919876543210      [Call Driver]                │ │
│ └─────────────────────────────────────────────────────────┘ │
│                                                             │
│ ┌─────────────────────────────────────────────────────────┐ │
│ │                    Live Map                             │ │
│ │                                                         │ │
│ │    📍 Pickup Point                                      │ │
│ │         │                                               │ │
│ │         ●─────●─────🚛─────●─────●                      │ │
│ │                                 │                       │ │
│ │                           📍 Delivery Point             │ │
│ │                                                         │ │
│ │ Current Location: Highway NH-48, near Lonavala         │ │
│ │ Last Updated: 2 minutes ago                             │ │
│ └─────────────────────────────────────────────────────────┘ │
│                                                             │
│ ┌─────────────────────────────────────────────────────────┐ │
│ │ Timeline                                                │ │
│ │                                                         │ │
│ │ ✅ Shipment Created      - Jan 15, 10:00 AM             │ │
│ │ ✅ Driver Assigned       - Jan 15, 11:00 AM             │ │
│ │ ✅ Package Picked Up     - Jan 15, 2:00 PM              │ │
│ │ 🔄 In Transit           - Jan 15, 2:30 PM              │ │
│ │ ⏳ Out for Delivery     - Pending                       │ │
│ │ ⏳ Delivered            - Pending                       │ │
│ └─────────────────────────────────────────────────────────┘ │
│                                                             │
│ [Share Tracking Link] [Download Invoice] [Contact Support] │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

## Driver Mobile App Wireframes

### 1. Driver Login (Mobile)
```
┌─────────────────────┐
│    ☰  TrackAS  🔔   │
├─────────────────────┤
│                     │
│                     │
│      📱 Login       │
│                     │
│  Email              │
│  [_______________]  │
│                     │
│  Password           │
│  [_______________]  │
│                     │
│    [   Login   ]    │
│                     │
│  Forgot Password?   │
│                     │
│  Don't have account?│
│     Register        │
│                     │
│                     │
└─────────────────────┘
```

### 2. Driver Dashboard (Mobile)
```
┌─────────────────────┐
│  👤 John  📍 Online │
├─────────────────────┤
│                     │
│ Today's Summary     │
│ ┌─────────────────┐ │
│ │ Earnings: ₹1,250│ │
│ │ Trips: 3        │ │
│ │ Rating: 4.8⭐   │ │
│ └─────────────────┘ │
│                     │
│ Available Shipments │
│ ┌─────────────────┐ │
│ │ TRK001          │ │
│ │ Electronics     │ │
│ │ 📍 2.5 km away  │ │
│ │ ₹850 earnings   │ │
│ │ [Accept] [View] │ │
│ └─────────────────┘ │
│                     │
│ ┌─────────────────┐ │
│ │ TRK002          │ │
│ │ Furniture       │ │
│ │ 📍 5.2 km away  │ │
│ │ ₹1,200 earnings │ │
│ │ [Accept] [View] │ │
│ └─────────────────┘ │
│                     │
│ [🏠] [📦] [💰] [👤] │
└─────────────────────┘
```

### 3. Active Shipment (Mobile)
```
┌─────────────────────┐
│  ← TRK123456789     │
├─────────────────────┤
│                     │
│ Status: Picked Up   │
│ ETA: 45 minutes     │
│                     │
│ ┌─────────────────┐ │
│ │                 │ │
│ │   🗺️ Map View   │ │
│ │                 │ │
│ │  📍 You are here│ │
│ │      │          │ │
│ │      ●──────●   │ │
│ │           📍    │ │
│ │      Destination│ │
│ └─────────────────┘ │
│                     │
│ Delivery Address:   │
│ 456 Delivery Ave    │
│ Pune, MH 411001     │
│                     │
│ Contact: Jane Smith │
│ 📞 +919876543211    │
│                     │
│ [📞 Call] [🧭 Navigate]│
│                     │
│ [Mark as Delivered] │
│                     │
│ [🏠] [📦] [💰] [👤] │
└─────────────────────┘
```

### 4. Proof of Delivery (Mobile)
```
┌─────────────────────┐
│  ← Proof of Delivery│
├─────────────────────┤
│                     │
│ TRK123456789        │
│                     │
│ Delivered to:       │
│ Jane Smith          │
│                     │
│ ┌─────────────────┐ │
│ │                 │ │
│ │   📷 Take Photo │ │
│ │   of Package    │ │
│ │                 │ │
│ │   [📸 Camera]   │ │
│ │                 │ │
│ └─────────────────┘ │
│                     │
│ ┌─────────────────┐ │
│ │  ✍️ Signature   │ │
│ │                 │ │
│ │  [Sign Here]    │ │
│ │                 │ │
│ └─────────────────┘ │
│                     │
│ Notes (Optional):   │
│ [_______________]   │
│                     │
│ [Complete Delivery] │
│                     │
│ [🏠] [📦] [💰] [👤] │
└─────────────────────┘
```

## Customer Tracking Interface

### 1. Public Tracking Page
```
┌─────────────────────────────────────────────────────────────┐
│                        TrackAS                              │
│                    Track Your Shipment                      │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│ Enter Tracking Number:                                      │
│ [TRK123456789________________] [Track]                      │
│                                                             │
│ ┌─────────────────────────────────────────────────────────┐ │
│ │ Shipment Status: In Transit                             │ │
│ │ Expected Delivery: Today, 6:00 PM                       │ │
│ │                                                         │ │
│ │ From: Mumbai, MH                                        │ │
│ │ To: Pune, MH                                            │ │
│ │                                                         │ │
│ │ ┌─────────────────────────────────────────────────────┐ │ │
│ │ │                Live Tracking                        │ │ │
│ │ │                                                     │ │ │
│ │ │    📍 Mumbai                                        │ │ │
│ │ │         │                                           │ │ │
│ │ │         ●─────●─────🚛─────●─────●                  │ │ │
│ │ │                                 │                   │ │ │
│ │ │                           📍 Pune                   │ │ │
│ │ │                                                     │ │ │
│ │ │ Current: Highway NH-48, near Lonavala               │ │ │
│ │ │ Last Updated: 2 minutes ago                         │ │ │
│ │ └─────────────────────────────────────────────────────┘ │ │
│ │                                                         │ │
│ │ Timeline:                                               │ │
│ │ ✅ Order Confirmed    - Jan 15, 10:00 AM               │ │
│ │ ✅ Picked Up          - Jan 15, 2:00 PM                │ │
│ │ 🔄 In Transit         - Jan 15, 2:30 PM                │ │
│ │ ⏳ Out for Delivery   - Pending                         │ │
│ │ ⏳ Delivered          - Pending                         │ │
│ │                                                         │ │
│ │ Driver: John Doe                                        │ │
│ │ Phone: +919876543210                                    │ │
│ │ Vehicle: MH01AB1234                                     │ │
│ └─────────────────────────────────────────────────────────┘ │
│                                                             │
│ [📱 Get SMS Updates] [📧 Email Notifications] [❓ Help]     │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### 2. Rating Interface
```
┌─────────────────────────────────────────────────────────────┐
│                        TrackAS                              │
│                   Rate Your Experience                      │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│ Shipment TRK123456789 has been delivered successfully!     │
│                                                             │
│ ┌─────────────────────────────────────────────────────────┐ │
│ │ How was your delivery experience?                       │ │
│ │                                                         │ │
│ │ Driver: John Doe                                        │ │
│ │ Vehicle: MH01AB1234                                     │ │
│ │                                                         │ │
│ │ Rating: ⭐ ⭐ ⭐ ⭐ ⭐                                      │ │
│ │                                                         │ │
│ │ Comments (Optional):                                    │ │
│ │ ┌─────────────────────────────────────────────────────┐ │ │
│ │ │ Great service! Package delivered on time and in    │ │ │
│ │ │ perfect condition. Driver was very professional.   │ │ │
│ │ │                                                     │ │ │
│ │ └─────────────────────────────────────────────────────┘ │ │
│ │                                                         │ │
│ │ [Submit Rating]                                         │ │
│ └─────────────────────────────────────────────────────────┘ │
│                                                             │
│ [Track Another Shipment] [Download Invoice]                │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

## Responsive Design Breakpoints

### Mobile (320px - 768px)
- Single column layout
- Collapsible navigation
- Touch-friendly buttons (min 44px)
- Simplified forms
- Bottom navigation for mobile apps

### Tablet (768px - 1024px)
- Two-column layout where appropriate
- Sidebar navigation
- Larger touch targets
- Optimized for both portrait and landscape

### Desktop (1024px+)
- Multi-column layouts
- Full sidebar navigation
- Hover states and interactions
- Keyboard navigation support
- Dense information display

## Accessibility Features

### WCAG 2.1 AA Compliance
- Color contrast ratio minimum 4.5:1
- Keyboard navigation support
- Screen reader compatibility
- Focus indicators
- Alt text for images
- Semantic HTML structure

### Internationalization
- RTL language support
- Unicode character support
- Locale-specific date/time formats
- Currency formatting
- Number formatting

### Performance Considerations
- Lazy loading for images
- Progressive web app features
- Offline functionality
- Fast loading times (<3 seconds)
- Optimized for low-bandwidth connections

## Component Library

### Buttons
```css
.btn-primary {
  background: var(--primary-600);
  color: white;
  padding: var(--space-3) var(--space-6);
  border-radius: 8px;
  font-weight: var(--font-medium);
  transition: all 0.2s ease;
}

.btn-primary:hover {
  background: var(--primary-700);
  transform: translateY(-1px);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
}
```

### Cards
```css
.card {
  background: white;
  border-radius: 12px;
  padding: var(--space-6);
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
  border: 1px solid var(--gray-200);
  transition: all 0.2s ease;
}

.card:hover {
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
  transform: translateY(-2px);
}
```

### Form Elements
```css
.form-input {
  width: 100%;
  padding: var(--space-3) var(--space-4);
  border: 1px solid var(--gray-300);
  border-radius: 8px;
  font-size: var(--text-base);
  transition: all 0.2s ease;
}

.form-input:focus {
  outline: none;
  border-color: var(--primary-500);
  box-shadow: 0 0 0 3px rgba(14, 165, 233, 0.1);
}
```

### Status Indicators
```css
.status-badge {
  display: inline-flex;
  align-items: center;
  padding: var(--space-1) var(--space-3);
  border-radius: 9999px;
  font-size: var(--text-sm);
  font-weight: var(--font-medium);
}

.status-success {
  background: var(--success-50);
  color: var(--success-700);
}

.status-warning {
  background: var(--warning-50);
  color: var(--warning-700);
}

.status-error {
  background: var(--error-50);
  color: var(--error-700);
}
```