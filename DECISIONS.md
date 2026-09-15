# Architectural & Product Decision Points

### Decision Point 1: Rejection Handling
* **Decision:** When a creator declines a booking request, the booking status updates to `Declined` on both the Creator Dashboard and Client Bookings views. The client sees the declined status along with an actionable "Explore Other Gigs" button that redirects them back to the marketplace.
* **Rationale:** This maintains operational transparency while keeping the user in the booking loop. Providing an immediate CTA to return to the marketplace prevents user drop-off and helps clients quickly find alternative creators for their project deadlines.

---

### Decision Point 2: Double Booking Strategy
* **Decision:** Allow multiple clients to send pending booking requests for the same gig simultaneously.
* **Rationale:** In a creator marketplace, creators often have high availability or capacity to fulfill multiple requests. Locking out potential clients while a request is merely pending creates artificial friction and reduces potential creator earnings. Slots or status locks should only occur once a creator explicitly accepts a booking.

---

### Decision Point 3: Marketplace Discovery & Ranking
* **Decision:** Implement a dynamic keyword search filter paired with category-based tag navigation.
* **Rationale:** Real-time client-side filtering provides instantaneous feedback for users searching for specific skills (such as AI Video or Scriptwriting). This ensures maximum visibility for newly posted gigs alongside established ones, giving equal discovery opportunities to all creators on the platform.
