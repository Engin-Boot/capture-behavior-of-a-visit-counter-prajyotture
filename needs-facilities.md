# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given Visitors are less on weekdays
  When The count of visitors is less compared to the weekends 
  Then Visitor Count is less on weekdays.

Scenario: Alert when seating capacity is full

  Given The Number of Tickets issued implies the capacity full
  When Number of Chairs in the halls are all occupied
  Then Then Alert "All Places Occupied" and capacity full.
