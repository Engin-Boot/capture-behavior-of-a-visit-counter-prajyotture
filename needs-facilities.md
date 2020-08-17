# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation 

Given Visitors are less on weekdays
  When Count is Less on weekdays compared to weekends.
  Then Visitor Count is less on weekdays.
  
Scenario: Alert when seating capacity is full

Given The Number of Tickets sold implies the capacity full. 
When Number of Chairs in the halls are all occupied
Then Alert "All Places Occupied" and capacity full.
