# Business Rules

## Appointments And Schedule

- An appointment can be created only within an active master shift.
- If a shift is absent, the master is unavailable for booking on the selected date.
- Two appointments for the same master must not overlap.
- Time slots shown to the client must be future slots only.
- Creating appointments in the past is allowed only for the administrator.
- Appointment duration is calculated from selected procedures and the master's duration coefficient.
- The minimum time slot step is 15 minutes.

## Workplace Limits

- Manicure and pedicure workplace limits are controlled separately.
- If the workplace limit is reached, creating another matching shift or appointment is blocked.
- The administrator can change workplace limits through salon settings.

## Materials

- After appointment completion, the system writes off materials according to service technology cards.
- Negative material stock is not allowed.
- If available stock is lower than the required usage norm, the system writes off available quantity and flags the issue.
- Only the administrator can manually change material stock.
- Repeated material write-off for the same appointment must be prevented.

## Appointment Statuses

- Appointment statuses are: new, confirmed, finished, cancelled and no-show.
- Finished, cancelled and no-show are final statuses.
- Finished appointments are used for revenue, payroll, KPI, loyalty and material write-off.
- Cancelled and no-show appointments are excluded from completed-visit calculations.

## Promo Codes And Loyalty

- A promo code can be applied only if it is active, valid by date and within usage limits.
- Loyalty discount is calculated from completed visits.
- Promo code and loyalty discount are not summed.
- If a discount is greater than the appointment cost, the final amount must not become negative.

## Access Control

- The master can access only own shifts, appointments and payroll data.
- The client can access only own appointments and personal cabinet data.
- Administrative settings, financial analytics and other employees' data are restricted from non-administrator roles.
- Deleting services or masters with active appointments is restricted.
