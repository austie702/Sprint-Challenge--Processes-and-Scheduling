## Multiple Choice and Short Answer Questions

1. List all of the main states a process may be in at any point in time on a
   standard Unix system. Briefly explain what each of these states mean.

   > * Created: Initialized but not yet in ready state.
   > * Ready/Waiting: Loaded into RAM but not executed.
   > * Running: Executed by the CPU or Kernel.
   > * Blocked: If an external trigger is needed.
   > * Terminated: Finished execution or been purponsely ended.

2. What is a Zombie Process? How does it get created? How does it get destroyed?
   > * A process that has been ended but remains on the process table until its parent process reads its exit status and finalizes its termination.  

3. Describe the job of the Scheduler in the OS in general.
   > * The scheduler's job is to vet every process requesting CPU time, and designate the amount of time it gets, based on several factors. 

4. Describe the benefits of the MLFQ over a plain Round-Robin scheduler.
   > * Round robin makes regular check-ins with every process on the list, looping in an unchanging cycle between the lot of them. Instead, MLFQ makes checks on processing requirements and status changes in real timme, adjusting their priority level if they require more or less processing power. 