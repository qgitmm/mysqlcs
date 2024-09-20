[Back](README.md)
# Select
```
  SELECT P.Name FROM Patient P
```

# Select with inner join
```
  --Select patients with appointments in the last 30 days.

  SELECT P.Name, A.ScheduledDate
  FROM Patient P
  JOIN Appointments A ON A.PatientId = P.id
  WHERE CONVERT(GETDATE(), VARCHAR, 111) >= CONVERT(DATEADD(d, -30 GETDATE(), VARCHAR, 111)
```

# Select with left(outer) join
```
  --Select patients for the last 30 days regardless if they had an appointment or not.

  SELECT P.Name, A.ScheduledDate, CASE WHEN A.Id IS NULL THEN 'Appointment Scheduled' ELSE 'No Appointment' END AS IsAppointmentScheduled
  FROM Patient P
  LEFT JOIN Appointments A ON A.PatientId = P.id
  WHERE CONVERT(GETDATE(), VARCHAR, 111) >= CONVERT(DATEADD(d, -30 GETDATE(), VARCHAR, 111)
```
