# System Architecture

The information system is implemented as a Laravel 12 web application.

## Architectural Approach

The application follows the MVC approach:

- models represent database entities and relationships;
- controllers process HTTP requests, validation and user actions;
- Blade templates form the user interface.

The application is divided into user areas:

- administrator panel;
- master cabinet;
- client cabinet;
- public online booking flow.

## Data Layer

The project uses MySQL and Eloquent ORM. Main models include:

- `Booking`;
- `Client`;
- `Master`;
- `Service`;
- `Material`;
- `MaterialMovement`;
- `Schedule`;
- `PromoCode`;
- `SalonSetting`;
- `User`.

Many-to-many relationships are represented through `booking_service`, `material_service` and `master_service`.

## Access Control

Role-based access is implemented for administrator, master and client workflows. The project materials describe use of Laravel middleware and Spatie Laravel Permission.

## Business Logic

Repeated business operations are separated into services, including material write-off, KPI calculation and report preparation. Appointment status changes trigger related operations such as material write-off and analytics updates.
