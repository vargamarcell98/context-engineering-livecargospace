🧠 PLANNING.md

🧰 Project Title

Live Freight Visibility Platform – Minimal working product for carriers and forwarders with real-time cargo space sharing via Gantt & map view.


---

🚛 Core Functionalities

Carrier View

Minimal CRM to manage:

Registered trucks (with capacity, plate number)

Saved clients / shippers (billing info, contact data)


Manual Load Registration, including:

Pickup & delivery address (country, ZIP, city, street, number)

Pickup & delivery time (date, hour, minute)

Total weight

Total cargo length (how much space the load occupies)

Assigned truck (selectable from registered ones)

Optional: notes, reference numbers, contact info, shipper (selectable from saved clients or entered manually)


Live Gantt Chart View of all planned loads, organized per vehicle

Live Map View with position updated every ~5 minutes via vehicle telematics API

Rest periods editable directly on the Gantt chart by clicking and selecting a time range (these are non-moving intervals)


Supplier / Forwarder View

No CRM or vehicle management

Live Gantt & Map View of all shared carrier capacity, showing:

Country and ZIP of pickup & delivery

Pickup & delivery time

Reserved cargo length and weight


They do not see company name, contact, or street address

Their value: aggregated live capacity from both their existing carrier partners and others using the platform → opportunity to match loads with unknown carriers



---

🔗 Data Sources & Flow

Vehicle positions: via API from external telematics provider (updated every 5 min)

All other data (loads, trucks, clients): entered manually by the carrier

Access control:

Suppliers/forwarders only see what carriers share publicly or with them

No direct communication yet (no chat, call, or bidding in MVP)




---

📱 Platforms

Optimized for mobile and desktop use

Built in Next.js + Supabase



---

✅ Scope Notes

No auto-matching or filtering logic for now

No bidding or rate negotiation yet

Focus: fast MVP that showcases live shared capacity

📎 UI Reference:
See [GANTT_UI_REFERENCE.png](./examples/GANTT_UI_REFERENCE.png) for the current prototype of the Gantt view created in Lovable.


