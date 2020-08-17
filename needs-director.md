# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given Patients comes in with relatives or friends
  When Patient enters assign him a special patient ID
  Then Every time patient comes in it updates the patient count
  and not relatives and friends.

Scenario: Compute parking slots to reserve for visiting specialists

  Given Special Parking Facilities is available
  When Visiting specialist Comes in assign him ticket for that parking slot
  and update parking counter
  Then parking slot is occupied and update total count of occupied 
  parking slots
