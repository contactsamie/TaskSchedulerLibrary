TaskSchedulerLibrary
====================

Task Scheduling Module for running a method or code base in scenarios that would have Traditionally been done by something like cron. Very usefull when you you are hosting your website with a web hosting company and you need a schedule task to run



1.   Implement the abstract class AbstractScheduledTask eg "SampleTask : AbstractScheduledTask" then write your code inside the Execute method

 
you can call the static class like this to run SampleTask's Execute method  after 10 min 

2.   ScheduleUtilityFactory.AddScheduleTaskToBatch(new SampleTask(" ONE ")
 {
             ScheduledTime = DateTime.Now.AddMinutes(10)
 });


and you are done!

