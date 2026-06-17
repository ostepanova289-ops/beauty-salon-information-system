# Analytics And KPI

The analytics module is used for monitoring salon performance and preparing management reports.

## Dashboard Metrics

- total revenue;
- average check;
- number of appointments;
- cancellation and no-show rate;
- master workload;
- revenue dynamics;
- booking status distribution;
- best KPI;
- master with maximum revenue for the selected period.

## Master Payroll

Payroll is calculated only from completed appointments:

```text
Payroll = Appointment amount * (payout_percent / 100)
```

The appointment amount includes the main service, additional services and applied discount logic.

## Master Workload

Workload is calculated by comparing occupied hours with scheduled working hours:

```text
Workload (%) = Occupied hours / Working hours * 100
```

Occupied hours are based on completed appointment duration. Working hours are calculated from shifts, excluding breaks.

## Reports

The system supports reports by:

- revenue;
- masters;
- services;
- materials;
- client appointments;
- loyalty program.

Reports can be filtered by period, master, service and appointment status. Export is available in PDF and Excel.
