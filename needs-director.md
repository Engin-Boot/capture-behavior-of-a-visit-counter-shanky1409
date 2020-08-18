# Visit-counter for a Director

## Scenario: Show patient visits during working days and holidays

  Given the system is running

  When I check the patient visit record

  Then display total patient visited hospital during working days and holidays

## Scenario: Compute parking slots to reserve for visiting specialists

  Given the number of specialist visiting the hospital on a day

  When the specialist arrives hospital

  Then the total designated parking should be available
