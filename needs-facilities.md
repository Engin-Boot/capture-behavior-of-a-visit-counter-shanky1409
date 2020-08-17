# Visit-counter for a Facilities Manager

## Scenario: Report visitor trends during a week of operation

  Given the sensor is running
  
  When I see the visitor trend report
  
  Then display the visitors for each day in the current week

## Scenario: Alert when seating capacity is full

  Given the sensor is running

  When the seating capacity gets full

  Then I get an alert message with capacity full
