##2014-11-18 Report
### Work Done
- Runtime of Jobs/Tasks
- Machine Avaiblility 
  - Attributes are obfusicated: We might need to makes some educated guesses
  - Failure rates: This can help us in failure prediction/modelling
- Task Requests: Using the task resource requests and machine availability, we can check whether over provisioning is actually true.


<img src="/job_event.jpg">

###Challenges
- Data is 217GB. We have still not run into any problems but we would like to prepare ourselves.
- Plan to tranfer the tables that we build into a DB so that join operations are easy


###TODO:
- Two more tables to look at
- Start looking at publications to see if they produce some result. This would help us validating our results. 

##2014-11-25 Report
##Pending from next week
Last weeks TODO

##Work Done
- Find the number of jobs running a given time instant
- Idea was to find if there is any periodicity in the data
- Plotted busy figures. Looks like there are some patterns.
<img src="/plot.png">
<img src="/plot1.png">

##Ideas
- Just take a slice of a day to see atleast daily periodicity
- Should I try smoothing?

##Challenges
- Ran out of memory. Tried subsampling and it worked! (Any other ideas?)
- matplotlib is not a good tool to plot graphs with large number of data points
- gnuplot was the next best option for me. Even she revolted!
- Again subsampling! sed is a good tool to use. (I think "El Presidente" mentioned it during his presentation!)
- Used pypy. I would encourage all to use it...it's fast!!

##TODO
- Good news...we have more data. Google just released a new column of the data. They claim "The new data is a randomly-picked 1 second sample of CPU usage from within the associated 5-minute usage-reporting period for that task. Using this data, it will be possible to build up a stochastic model of task utilization over time for long-running tasks."

