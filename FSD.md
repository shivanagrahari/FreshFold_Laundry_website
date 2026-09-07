# Laundry Service Website — Functional Specification Document (FSD)

## 1. Document Overview
**Project:** Laundry Service Website  
**Version:** 1.0  
**Status:** Ready for UI/UX and MVP development  
**Data:** Dummy data initially; business data can be replaced later.

## 2. Objective
Build a modern, responsive laundry-service website that helps customers discover services, view pricing, schedule doorstep pickup, understand the process, and contact the business. The initial release uses dummy business information and is structured so production data can be substituted easily.

## 3. Target Users
- Residential customers
- Students and working professionals
- Families
- Businesses requiring recurring laundry
- Customers looking for dry cleaning/ironing

## 4. Website Scope
### Public Pages
1. Home
2. Services
3. Pricing
4. How It Works
5. About Us
6. FAQs
7. Contact / Book a Pickup
8. Terms & Conditions
9. Privacy Policy

### Future Modules
- Customer login/signup
- Order tracking
- Customer dashboard
- Subscription plans
- Coupon management
- Admin dashboard
- Delivery partner dashboard
- Online payment integration
- WhatsApp automation
- Order status notifications

## 5. Home Page Requirements
### Header
- Logo / brand name
- Navigation: Home, Services, Pricing, How It Works, About, FAQ, Contact
- Primary CTA: Book a Pickup
- Mobile hamburger navigation

### Hero
- Strong headline
- Supporting text
- Book a Pickup CTA
- View Services CTA
- Trust indicators

### Service Highlights
- Wash & Fold
- Wash & Iron
- Dry Cleaning
- Steam Ironing
- Household Laundry
- Delicate Care

### How It Works
Four steps:
1. Book
2. Pickup
3. Clean
4. Deliver

### Benefits
- Doorstep convenience
- Professional cleaning
- Hygienic handling
- Transparent pricing
- On-time delivery
- Easy booking

### Pricing Preview
Show popular services and starting prices with link to full pricing.

### Testimonials
Show customer name, locality, rating and review.

### Service Areas
Show supported dummy locations.

### FAQ Preview
Show common questions with expandable answers.

### Final CTA
Encourage users to schedule a pickup.

## 6. Services Page
Each service shall contain:
- Service name
- Description
- Typical turnaround
- Starting price
- CTA to book

## 7. Pricing Page
Pricing shall support:
- Per kg pricing
- Per item pricing
- Service category
- Starting price
- Optional express-service surcharge
- Notes about final pricing

Dummy examples:
- Wash & Fold: ₹79/kg
- Wash & Iron: ₹109/kg
- Shirt Ironing: ₹15/item
- Dry Cleaning: ₹149/item
- Bedsheet: ₹99/item
- Blanket: ₹249/item

## 8. Booking Flow
### Step 1 — Customer Details
- Full name
- Mobile number
- Email (optional)

### Step 2 — Pickup Details
- Address
- Landmark
- Preferred pickup date
- Preferred time slot

### Step 3 — Service
- Service type
- Approximate quantity
- Special instructions

### Step 4 — Confirmation
Display:
- Booking reference
- Pickup date/time
- Selected service
- Estimated amount
- Contact information

For the MVP, submission may show a confirmation message without a backend.

## 9. Contact Page
Fields:
- Name
- Phone
- Email
- Subject
- Message

Also display dummy:
- Phone
- Email
- Address
- Business hours
- WhatsApp CTA

## 10. FAQ
Initial questions:
- How does pickup work?
- How long does laundry take?
- Is same-day service available?
- How is pricing calculated?
- Do you handle delicate clothes?
- What payment methods are accepted?
- What happens if a garment is damaged?

## 11. Non-Functional Requirements
### Responsive Design
Support:
- Mobile: 320px+
- Tablet: 768px+
- Desktop: 1024px+
- Large desktop: 1440px+

### Performance
- Lightweight static assets
- No unnecessary libraries
- Lazy loading for non-critical imagery
- Minified production assets when deployed

### Accessibility
- Semantic HTML
- Keyboard-accessible controls
- Visible focus states
- Form labels
- Sufficient text contrast
- Alt text for meaningful images

### SEO
- Unique page title
- Meta description
- Semantic headings
- Open Graph metadata
- Local-business schema can be added after real business details are available
- Sitemap and robots.txt for production

## 12. UI/UX Direction
### Visual Style
Clean, premium, trustworthy and friendly.

### Suggested Palette
- Primary: Deep navy
- Secondary: Aqua/blue
- Accent: Fresh green
- Background: Off-white
- Text: Dark slate

### Typography
Use a modern sans-serif such as Inter/system font stack.

### UX Principles
- Primary CTA always easy to find
- Short forms
- Clear pricing
- Mobile-first booking
- Strong trust signals
- Consistent cards and spacing
- Sticky mobile booking CTA

## 13. Form Validation
- Required fields must be validated client-side.
- Phone number must contain a valid Indian mobile format in the demo.
- Invalid email must show an inline message.
- Pickup date cannot be earlier than today.
- Successful booking displays a unique demo reference.

## 14. Analytics Events — Production Ready
Recommended events:
- book_pickup_click
- service_view
- pricing_view
- booking_started
- booking_submitted
- contact_submitted
- whatsapp_click
- phone_click

## 15. Security
For production backend:
- Server-side validation
- Rate limiting
- CSRF protection where applicable
- Secure authentication
- HTTPS
- No sensitive information stored in client-side code
- Payment handled through a PCI-compliant provider

## 16. Acceptance Criteria
- Website loads correctly on mobile, tablet and desktop.
- Navigation works on all pages.
- All primary CTAs work.
- Services and pricing are readable.
- Booking form validates required data.
- Successful demo booking generates a confirmation reference.
- Contact form validates inputs.
- FAQ accordion works.
- No horizontal overflow at common viewport widths.
- Website contains no broken internal links.
- Dummy data is clearly replaceable with production data.

## 17. Dummy Business Data
**Brand:** FreshFold Laundry  
**Tagline:** Fresh Clothes. Zero Hassle.  
**Phone:** +91 98765 43210  
**Email:** hello@freshfold.example  
**Location:** Pune, Maharashtra  
**Hours:** Mon–Sun, 8:00 AM–9:00 PM  
**Service Area:** Pune & selected nearby areas

## 18. Future Admin Data Model
Core entities:
- Customer
- Address
- Service
- Price
- Booking
- BookingItem
- PickupSlot
- Payment
- Coupon
- DeliveryPartner
- Notification
- Review

## 19. Release Plan
### MVP
Public website + responsive UI + client-side booking/contact demo.

### Phase 2
Backend + database + admin panel + real booking management.

### Phase 3
Payments + delivery tracking + customer accounts + notifications.

### Phase 4
Subscriptions + loyalty + analytics + automated marketing.
