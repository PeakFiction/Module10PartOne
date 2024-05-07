## Reflection

### Experiment 1.2:

The reason why the "hey there" message comes first before the "howdy" and "done" is because the lines that print out "hey there" are placed before the executor. "Howdy" and the "done" messages are printed out after the executor is run.
<img width="515" alt="Screenshot 2024-05-07 at 12 19 47" src="https://github.com/PeakFiction/Module10PartOne/assets/112671939/ff17767d-ab77-49eb-a787-4b173956b055">
<img width="499" alt="Screenshot 2024-05-07 at 12 19 58" src="https://github.com/PeakFiction/Module10PartOne/assets/112671939/26a50219-4594-423b-a75a-d04cae9f02c9">


### Experiment 1.3:

#### Spawner
How it works is the executor.run() uses a while loop that iterates through its instructions that were spawned in, and then initiated them. Since there are multiple, it didn't need to wait for one task to complete before starting the next. This is why it can initiate all 3 tasks asynchronously, i.e. printing all howdies at once. And then after 2 seconds, it prints out all the done's.

#### Drop Spawner
From what I see, the program isn't terminating once everything's done and dusted. The reason why is because there's still a thread holding the spawner that is keeping it. If the drop(spawner) isn't there, the thread will continue to run.