# Admin Documentation & Usage Information

## 1. Bookings Management

Use the bookings management area to view and manage all customer bookings. Bookings can be confirmed or cancelled, and the system automatically prevents double-booking for confirmed time slots.

### Available actions

- **Confirm**: Approves the booking and blocks the time slot in the calendar. This sends an automated email confirmation to the client.
- **Cancel**: Rejects the booking and frees up the time slot. This sends an automated cancellation email.
- **Delete Booking**: Safely removes the record from the Firestore database using a custom, iframe-friendly inline approval system to avoid native browser dialog issues.

## 2. Services & Provided Packages

Use the services and packages area to edit the packages shown on the homepage. You can change prices, descriptions, and feature lists.

### Current active services

- **Commuter Companion (CBT-Ready)**: Built for new riders who have passed their CBT and want confidence navigating their daily route.
- **Confidence Builder Session**: Concentrated practice on junctions, roundabouts, high-speed filtering, and real-world safe positioning.
- **Leisure & Scenic Ride**: Tailored group or solo rides exploring technical corners and country lanes with Dennis.

### Add a service

Create brand-new packages by entering the package details, price, and comma-separated feature lists.

## 3. Advanced AI Trip Planner

The proprietary generative motorcycle trip engine allows riders to plan complete custom tours.

### Integrated advanced functions

- **Adaptive Motorcycle Handling**: Customizes safety guidance, cornering speeds, and route styles dynamically according to whether the user rides a Cruiser, Sportbike, Adventure Tourer, Naked/Standard, or Commuter Scooter.
- **Pillion/Passenger Mode**: Modifies safety warnings and pacing calculations when carrying a passenger, advising on passenger weight transfer, cornering dynamics, and brake distance adjustments.
- **Persistent Route Archiving**: Integrates with Firestore so logged-in users can save generated trips and build a secure, private archive of custom-tailored itineraries.
- **Cost Calculation**: Estimates pricing in real time based on a £50/hour guiding base, plus optional £150/day bike rental and a £50/day passenger coaching premium.

## 4. Availability Calendar

Use the availability calendar to set which days and times are available to be booked.

### Calendar controls

- **Select Date**: Pick a date on the calendar. Dates with a dot have bookings.
  - Yellow dot: unconfirmed booking.
  - Black dot: the selected date has bookings.
- **Toggle Slots**: Click time slots to make them available. Available slots are shown in yellow. Click again to remove availability.
- **Save**: Click **Save Availability** for changes to take effect on the frontend.

## 5. Live Chat

Use live chat to respond to website visitor messages in real time.

- Messages are visible to anyone on the site, allowing admins to answer general queries quickly.
- Admin messages are highlighted to distinguish them from user messages.

## 6. Email Notifications

The system is configured to send email alerts to `dennismark2603@gmail.com` whenever:

- A new booking is requested.
- A new message is sent in the live chat by a user.
