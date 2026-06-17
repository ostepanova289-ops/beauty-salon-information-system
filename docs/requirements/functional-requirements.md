# Functional Requirements

## Online Booking

- The system must allow clients to create online appointments through a web interface.
- The system must support booking without mandatory registration.
- The system must allow choosing a main service, additional services, a master, date and free time.
- The system must support choosing a specific master or an automatic "any available master" option.
- The system must calculate appointment duration from selected services and the master's duration coefficient.
- The system must calculate appointment cost using service prices and the master's price coefficient.
- The system must send a notification after appointment creation when contact data is available.

## Schedule And Workplaces

- The system must store masters' shifts, working time and breaks.
- The system must show only free time slots within active shifts.
- The system must check existing appointments before creating or editing a booking.
- The system must control separate limits for manicure and pedicure workplaces.
- The system must prevent creation of shifts or appointments that exceed workplace constraints.

## Appointments

- The system must support appointment statuses: new, confirmed, finished, cancelled and no-show.
- The system must use the finished status as the trigger for material write-off, payroll calculation and analytics updates.
- The system must exclude cancelled and no-show appointments from completed-visit calculations.

## Clients, Loyalty And Promo Codes

- The system must store client contact data and visit history.
- The system must calculate loyalty discounts from completed visits.
- The system must support promo codes with activity status, validity period and usage limits.
- The system must avoid combining promo code and loyalty discounts.

## Services And Materials

- The system must maintain a service catalog.
- The system must support main and additional services.
- The system must store allowed combinations of main and additional services.
- The system must maintain material stock records.
- The system must connect services with materials through technology cards.
- The system must automatically write off materials after appointment completion.
- The system must keep a history of material movements.

## Payroll, KPI And Reports

- The system must calculate master payroll from completed appointments and individual payout percentage.
- The system must calculate revenue, average check, workload, cancellations and KPI indicators.
- The system must provide filters by period, master, service and appointment status.
- The system must generate management reports.
- The system must export reports to PDF and Excel.
