---
layout: default
title: Exams
---

<table id="customers">
  <tr>
    <th> # </th>
    <th>Topic</th>
    <th>Date</th>
    <th>Skillset</th>
    <th>Cheat Sheet</th>
    <th>Sample 1</th>
    <th>Sample 2</th>
    <th>Exam & Solutions</th>
  </tr>
  {% for iteml in site.data.exam %}  
    {% assign item = iteml[1] %}
    <tr>
        <td>{{ item.num }}</td>
        <td> {{ item.topic }} </td>
        <td> {{ item.date | date: "%b %d" }} </td>
        <td> 
        <!-- Skillset  -->
            {% if item.skillset %}
            <a href="{{ site.base }}{{ item.skillset }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="{{ iteml[0] }} skillset"
                    title="{{ iteml[0] }} skillset"
                    src="{{ site.base }}/img/icons/notes.png" />
            </a>
            {% endif %}
        </td>
        <td> 
        <!-- Cheatsheet  -->
            {% if item.cheat_sheet %}
            <a href="{{ site.base }}{{ item.cheat_sheet }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="{{ iteml[0] }} cheat sheet"
                    title="{{ iteml[0] }} cheat sheet"
                    src="{{ site.base }}/img/icons/cheat_sheet_icon.png" />
            </a>
            {% endif %}
        </td>
        <td> 
        <!-- Sample Exam 1 -->
            {% if item.samp_exam1 %}
            <a href="{{ site.base }}{{ item.samp_exam1 }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="{{ iteml[0] }} sample exam"
                    title="{{ iteml[0] }} sample exam"
                    src="{{ site.base }}/img/icons/lab_questions.png" />
            </a>
            {% endif %}
            {% if item.samp_exam2_sol %}
            <a href="{{ site.base }}{{ item.samp_exam1_sol }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="{{ iteml[0] }} exam solutions"
                    title="{{ iteml[0] }} exam solutions"
                    src="{{ site.base }}/img/icons/lab_solutions.png" />
            </a>
            {% endif %}              
        </td>
        <td>
        <!-- Sample Exam 2 -->
            {% if item.samp_exam2 %}
            <a href="{{ site.base }}{{ item.samp_exam2 }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="{{ iteml[0] }} sample exam"
                    title="{{ iteml[0] }} sample exam"
                    src="{{ site.base }}/img/icons/lab_questions.png" />
            </a>
            {% endif %}
            {% if item.samp_exam2_sol %}
            <a href="{{ site.base }}{{ item.samp_exam2_sol }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="{{ iteml[0] }} exam solutions"
                    title="{{ iteml[0] }} exam solutions"
                    src="{{ site.base }}/img/icons/lab_solutions.png" />
            </a>
            {% endif %}            
        </td>        
        <td> 
            {% if item.exam_questions %}
            <a href="{{ site.base }}{{ item.exam_questions }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="{{ iteml[0] }} exam questions"
                    title="{{ iteml[0] }} exam questions"
                    src="{{ site.base }}/img/icons/lab_questions.png" />
            </a>
            {% endif %}
            {% if item.exam_solutions %}
            <a href="{{ site.base }}{{ item.exam_solutions }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="{{ iteml[0] }} exam solutions"
                    title="{{ iteml[0] }} exam solutions"
                    src="{{ site.base }}/img/icons/lab_solutions.png" />
            </a>
            {% endif %}
        </td>
    </tr>        


  {% endfor %}

</table>



&nbsp;

Couple things to note about exams:
- All the midterms will be administered during lecture time on Zoom. 
- There will be no final. The final exam periods is for conflicts given to students with documented medical emergencies.  

### Exam Policies

Besides the obvious "don't cheat" exam policies outlined in the [policies page](/policies/cheating), you should know about the following exam procedures: 

#### Summer exam testing procedure

Since many of the summer students will be taking the course online, the exam policy needs to be slightly modified. Hence, exams will still be done synchronously on their assigned date at 10AM, but must be taken online over Zoom wherever you are. We will proctor through Zoom and at the end of the session you can upload your exam to Gradescope. So online students must make arrangements to set up a Zoom-enabled device monitoring a clear workspace.


#### Exam conflicts

Exam conflict will be offered at the end of the semester during the final period. You are eligible to take the conflict exam **only if you have a documented emergency with prior authorization of the emergency dean and course instructor**.


#### Cheatsheet

I've wrestled with the concept of cheatsheets a lot in past semesters. Ideally, what a cheatsheet is for is to help you memorize tedious equations or details that are easy to forget. However, I like to give exam questions that are very similar to the HWs/labs. In prior semesters, I noticed that cheat sheets didn't contain definitions/algorithms. Instead, they contained copied questions and solutions of HW/lab problems. Basically, cheat sheets had become a "guess what Kani might put on the exam"-sheet. Worse, many, many people simply copied the cheatsheet solutions and were frustrated when they learned that those solutions didn't apply to the exam problems. This leaves me with two options: 

- Make sure that the exam problems are changed up so that copying from an HW/lab problem would hurt more than help. 
- Eliminate cheatsheets altogether. 

I think I've come up with a solution that'd help everyone. Over the course of several semesters, we've constructed a communal cheat sheet for each of the exams. These cheat sheets will be posted on the website well in advance of the exam and will be attached to the back of the exam. 

This lets me use problems that many of you have seen before but know that the people answering those problems are doing so because they actually mastered the material. 

#### Use pen

The exams will be scanned and uploaded to Gradescope where they will be graded by the TAs. Unfortunately, last semester we had a problem with a number of individuals that used a pencil with a light touch causing the exam to be illegible. Therefore, we're banning pencils. I'm not going to go around confiscating pencils like some weird pen nazi, but if we see an exam that is difficult to read, we will take off points. Just use pen, if you need to change something you can always cross out the previous answer and make a note for the grader to look at the scratch page.  


### Regrades

Regrades requests would be open for a week once grades are released (unless it is infeasible due to grade submission time constraints). Regrade requests are not intended for arguing about point allocation or whether the grading scale is fair.

Unfortunately, certain students think that they can tire us into giving them points that they did not earn, by continuously asking for unjustified regrade requests. This is especially true in the case of exams. I have had students that would submit a grade request for **every single exam problem**, hoping for more points. That's not cool. As such, superfluous, argumentative, and repetitive regrade requests, after an appropriate warning, would result in a zero on the relevant questions - please do not waste our time.

Again, you should not fear submitting regrades if you have a question that you're confused and didn't gain any insight from the exam solutions (**please check the solutions first**). It's just that in any large group, there will be a few individuals who view teaching as an adversarial relationship and I have to make this stupid announcement for them. I hate it as much as you do. 
 
### DRES
- If you have a DRES accommodation, please email the course staff directly (not sure if sending documents over Piazza is compliant with EHR policies or not, but why risk it). Make sure I respond that I've recorded your accommodation! If I don't respond email again.
- Because of the limited staff, if you plan on using a DRES accommodation, you will need to take the exam at the [TAC](https://www.disability.illinois.edu/academic-accommodations-and-supports/academic-accommodations/testing-accommodations) synchronously with the rest of the class. We do not have the staff to manage accommodations ourselves. 
- Best thing you can do is to schedule the exams with TAC **now**. That way, there is no chance of forgetting to schedule a slot and missing out on your accommodations.  
