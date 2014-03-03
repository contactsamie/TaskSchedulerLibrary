TaskSchedulerLibrary
====================


http://visualstudiogallery.msdn.microsoft.com/a4a4f042-ffd3-42f2-a689-290ec13011f8


Task Scheduling Module for running a method or code base in scenarios that would have Traditionally been done by something like cron. Very usefull when you you are hosting your website with a web hosting company and you need a schedule task to run

A.   Implement the abstract class AbstractScheduledTask eg "SampleTask : AbstractScheduledTask" then

write your code inside the Execute method
 you can call the static class like this to run SampleTask's Execute method  after 10 min 

B.  ScheduleUtilityFactory.AddScheduleTaskToBatch(new SampleTask (DateTime.Now.AddMinutes(1), " RUN AFTER 10 MIN "));

and you are done!
 

