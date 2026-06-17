# Database Design

The project uses a relational database model. This model was selected because one appointment is connected with multiple business objects at the same time: client, master, service, schedule, materials, promo code and analytics.

## Design Principles

- Separate storage for clients, users, masters, services and materials.
- Foreign keys to preserve relationship integrity.
- Many-to-many tables for services, masters, bookings and material technology cards.
- Separate material movement history instead of storing only current stock.
- Separation of user accounts and salon client records.
- Extensibility for new modules through additional entities and relationships.

## Main Tables

| Table | Purpose |
| --- | --- |
| `users` | User accounts for administrators, masters and clients with personal cabinet access. |
| `clients` | Client database with contact data and administrator notes. |
| `masters` | Master profiles, coefficients, payout percentage and calendar color. |
| `bookings` | Central appointment table connected with client, master and main service. |
| `booking_service` | Additional services selected within one appointment. |
| `services` | Service catalog with duration, price and active/additional service flags. |
| `service_addons` | Allowed combinations of main and additional services. |
| `materials` | Material directory with current, minimum and critical stock levels. |
| `material_service` | Technology cards: materials and usage norms for services. |
| `material_movements` | History of restock, manual write-off and automatic write-off operations. |
| `schedules` | Masters' shifts with date, start/end time and breaks. |
| `master_service` | Services available to specific masters. |
| `promo_codes` | Promo code discount settings and usage limits. |
| `salon_settings` | Salon-level limits and booking rules. |

## ERD

![ERD database model](../../diagrams/erd/database-erd.jpeg)
