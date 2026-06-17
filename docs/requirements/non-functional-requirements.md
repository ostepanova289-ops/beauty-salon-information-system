# Non-Functional Requirements

## Architecture

- The system must be implemented as a web application.
- The system must use Laravel 12 and MySQL according to the project materials.
- The architecture must support centralized data storage and browser-based access.

## Adaptability

- The interface must work on devices with different screen sizes, including desktops, tablets and smartphones.

## Security

- Access to system sections must depend on the user's role.
- Passwords must be stored in hashed form.
- Internal salon data must be available only to authorized users with the required access level.
- Server-side validation must be used for input checks.

## Data Integrity

- The system must validate appointment time, master shift, breaks and workplace limits before saving appointment data.
- The system must prevent repeated material write-off for the same completed appointment.
- The system must maintain relational integrity between appointments, clients, masters, services, materials and schedules.

## Maintainability And Extensibility

- The system architecture must allow adding or changing salon settings and functional modules without redesigning the whole structure.
- Business logic used in several workflows should be separated from interface templates and reusable across modules.
