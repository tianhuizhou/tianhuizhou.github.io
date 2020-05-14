---
layout: project
type: project
image: images/Scheduling.jpg
title: Timetable
permalink: projects/Timetable
# All dates must be YYYY-MM-DD format!
date: 2020-01-21
labels:
  - Simulated Annealing Algorithm
  - C++
summary: Implementing Simulated Annealing Algorithm to solve an NP problem.
---

<div class="ui images">
  
  <img class="ui big right image" src="../images/Timetable.png">
</div>

<h2 id="overview">project-overview</h2>
The problem that we are trying to solve in this project is to automate the task of creating classroom timetables which is an NP problem. An NP problem is a hard problem that cannot be solved in polynomial time which is more difficult than problems that can be solved in polynomial time. This is important because it can save time for administrators to determine class schedules.

<h2 id="contribution">My Contribution</h2>
In this project, I complete the sequential version of the program. It can automate task of creating a timetable for input file. I implement Simulated Annealing Algorithm for doing the task.

I handle the problems that adding probabilities to accept "Bad Move".
<p><img class="ui large image" src="../images/TimetableResult.png" alt="result" /></p>

The program is able to read input files and output a timetable as csv file to show the details.
<p><img class="ui large image" src="../images/TimetableReport.png" alt="report" /></p>
Here is some code about Cost that how I calculate the cost:

```js
if (schedule[time_tem][loc_tem] >  1) { // clash in time&location
			if (schedule[row_tem][col_tem] == 0)
				dif_cost++;
		} else { //no clash
			if (schedule[row_tem][col_tem] > 0)
				dif_cost--;
		}
        
        if(row_tem != time_tem){
		if (schedule2[time_tem][index_teacher] > 1) { // there is a clash in time&teach
			if (schedule2[row_tem][index_teacher] == 0)
				dif_cost++;	
		} else {
			if (schedule2[row_tem][index_teacher] > 0) 
				dif_cost--;
		}
        }
```
In this project, I learned that how to work with other people as a team. Everyone in a group should take their own responsibilities and contribute their strengths to push forward the project. Furthermore, having quality and efficient communication with teammate is important because it can make sure everyone works on the same page and reduce producing error.

link of the code: <a href="https://github.com/ICSatKCC/TimeTablingProject"><i class="large github icon"></i>Timetable</a>


