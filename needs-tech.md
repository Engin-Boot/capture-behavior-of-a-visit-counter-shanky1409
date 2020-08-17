# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given that I restart the system
  When I check the total visit-count
  Then it should not refresh the count from 0

Scenario: Reconcile counts if the sensor is offline for a while

  Given the system is offline for a while
  When I check the total visit-count
  Then the count should be greater or equal to total visit before offline
