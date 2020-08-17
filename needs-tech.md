# Visit-counter technical needs

Scenario: Recover across restarts of the server that runs the visit-counter
Given The Server is good and running
When abruptly it fails due to operating system issues or network issues
Then restart the server without losing data

Scenario: Reconcile counts if the sensor is offline for a while

  Given The Server is running
  When There is Power failure it crashes or go down
  Then when power supply resumes reboot and start the 
  counter from where it was left with
