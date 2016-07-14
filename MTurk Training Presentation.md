class: center, middle

# An Introduction to Mechanical Turk for Survey Research 
### John Sperger
### July 14, 2016

---

# Agenda

1. What is Mechanical Turk and why use it? 
2. How to Post a Study on Mechanical Turk and Basic Considerations
3. Being a Responsible Requester 
4. Intermediate MTurking 
 * Designing Studies for Mechanical Turk
 * The Mechanical Turk API

---

class: center, middle

# What is Mechanical Turk and why use it? 

---

# What is Mechanical Turk (MTurk)?

Mechanical Turk is an online crowd sourcing platform created by Amazon. The site acts like a job board - Requesters can post jobs (Human Intelligence Tasks or HITs in MTurk parlance) which can be completed by Workers. 


Mechanical Turk is very popular with researchers in psychology because you can quickly collect survey responses for a low cost. Two of the most common use cases are pilot testing studies and study components and running high powered studies. 

The typical MTurk study is generally shorter and less complex than a lab study, but you can run longer and more complex studies and still get great data. 


---

# Why Use Mechanical Turk?

* It's quick - Collecting thousands of responses can take less than a day

* It's cheap - the going rate for survey responses on Mechanical Turk is $6/hr or 10 cents per minute (more on this later)

* Mechanical Turk will give you a more demographically diverse sample than the lab. You can also restrict your sample to certain geographic regions

* Workers on Mechanical Turk (MTurkers for short) seem to be at least as attentive as lab participants, if not more so, according to research done directly comparing attentiveness of MTurkers and lab participants

* MTurk studies are widely accepted and you can find them in all journals including top tier journals

---

# Mechanical Turk is Different than the Lab

You can't see what MTurkers are doing when they complete your survey. 

Requesters are not anonymous. Workers post reviews of requesters on forums and Reddit, and there is a browser plugin called TurkOpticon which overlays the requester's ratings onto MTurk. Maintaining a good rating helps you get high quality responses quickly. 

Professional Participant Pool. While nonnaïveté is also a problem for lab studies, a sizeable minority of MTurkers use MTurk as their primary source of income. This is doubly true when you add qualifications that workers have already completed X surveys. 
* Deception isn't as likely to work

There is cross-talk between participants. Usually the discussion is general and more about what studies and requesters are high paying rather than the details of a study, and on MTurk forums there are community norms that participants shouldn't talk about study manipulations. 
 * If you have a study that's annoying or pays poorly for the effort involved participants will probably post about it. 

---

class: center, middle

# Posting a HIT on Mechanical Turk and Basic Considerations

---

# Creating a New HIT

.image-75[![Create New Project](https://raw.githubusercontent.com/jsperger/MTurkForResearchers/master/Images/Create%20New%20Project.png)]

---

# New Project - Survey Link

.image-75[![New Project - Survey Link](https://raw.githubusercontent.com/jsperger/MTurkForResearchers/master/Images/New%20Project%20-%20Survey%20Link.png)]

---

# Components of a HIT - Description

.image-75[![Mturk Hit Description Example](https://raw.githubusercontent.com/jsperger/MTurkForResearchers/master/Images/HIT%20Description.png)]

Title - The title alone is what workers first see when looking for HITs; sentences instead of single words are the standard
* Typically you should include the estimated time to complete in the title of the HIT

Description - Give more detail about the task. 
* If your HIT contains the following you should mention it explicitly in the description: writing tasks, video watching, listening to audio

Keywords - keywords that workers can use to search for your HIT

---

# Providing Good Time Estimates

Providing accurate time estimates is one of the most important things you can do as a requester. 

* The average worker on Mechanical Turk probably reads more slowly than you do
* Keep in mind that you've seen your study materials before. Even if you try to read carefully you'll probably still end up skimming if you try to estimate the completion time for your own study
* Try asking a friend or someone in your lab group to give you a time estimate (This is also a good way to get feedback in general)

For short studies try to avoid giving a range of times. A "1-3 Minute Study" which pays fifteen cents could correspond to hourly wages of $9.00/hr, $4.50/hr, or $3.00/hr.

* Rule of Thumb: If a study is five minutes or less don't give a range. 

---

# Components of a HIT - The Set Up

.image-75[![HIT Set Up](https://raw.githubusercontent.com/jsperger/MTurkForResearchers/master/Images/HIT%20Set%20Up.png)]
 
Time alloted per assignment - this is *not* how long your HIT takes to complete. This is how long a worker has to complete the HIT before Amazon automatically prevents the worker from submitting the HIT and allows another worker to have a chance to complete the assignment. 

---

# Total Cost of an MTurk HIT

Reward per assignment
* MTurk standard is 10 cents/minute which works out to $6.00/hour
* We should do better - The Behavioral Lab pays participants $10/hr. The federal minimum wage is $7.25/hour . Paying less means you're more likely to get an economically vulnerbale segment of the population, and the costs are still significantly lower than other alternatives for collecting survey responses. 
* You'll get responses more quickly with higher pay, and past studies have found that higher base pay also increases response quality

Mechanical Turk charges a 40% fee for HITs which have more than 9 assignments. 
* The fee for HITs with fewer than 9 assignments is 20%
* The fee for bonuses is also 20%

Imagine you're running a study where you'll collect 100 responses for a five minute survey which you'll pay participants 70 cents to complete. The total cost would be (100)($.70)(1.4) = $98. 

---

# Components of a HIT - Worker Requirements

.image-75[![Worker Requirements](https://raw.githubusercontent.com/jsperger/MTurkForResearchers/master/Images/Worker%20Requirements.png)]

Master Workers - costs extra money and is basically useless provided you use sensible worker qualifications

Additional Qualifications - You can create your own qualifications and assign them to workers. This is very powerful. 
* You can screen out participants who have taken similar studies you have launched before

---

# Options for Confirmation

There are two main options for confirming that workers actually completed your survey

Payment Code - At the end of the survey give participants a payment code to enter in the text box when they submit the HIT on MTurk
* Easy to set up
* Errors - people accidentally submit the HIT before completing the survey or enter the wrong completion code (overall low error rate though)
* You can combine this with bonuses to create incentivized studies

External Question HIT - displays the survey automatically in a frame on within MTurk and automatically submits the HIT when they have completed the survey
* Workers can't accidentally submit the HIT before completing it 
* Can only be set up through the MTurk API 

---


class: center, middle

# Some Final Words Warning
## If you're using a completion code, double check it's working before launching your study!

### Want to get 100 emails in five minutes? Launch a study without a completion code

---

class: center, middle

# Being a Good Requester 

---

# The Basics of Being a Good Requester

Pay fairly 

Approve work promptly. If someone entered the wrong completion code check to see if you have a completed survey response matching the ID. 
* When using completion codes sometimes participants will accidentally submit the HIT with their MTurk ID as the completion code (The first survey question is usually "What is your MTurk ID?" and people copy and paste in the wrong window). This is fairly common - I'd estimate this happens once per 100-200 responses. 

Respond to messages from participants 

Be considerate when designing surveys
* Be cognizant of effort intensive tasks. A five minute survey which is actually five minutes of essay writing will make participants justifiably frustrated if you don't tell them up front


---

# Rejecting Work 

Be clear when rejecting work. My boiler plate reason for rejection is "Your work has been rejected because your completion code was incorrect and there are no completed surveys matching your MTurk ID"
* If you reject someone's work they will sometimes send you nasty emails. 
* While purely anecdotal evidence, I've noticed that some of the workers who submit the worst work will most aggressively message you to try to shame you into reversing the rejection. While rare (and I mean very rare in my experience), be aware that some people do adopt this strategy

---

# Cheating

If it looks like a lot of people are cheating, they probably aren't. In the past year of running the department's account I have collected ~150,000 survey responses. In that time I've had to block only three people for deliberate attempts to cheat.

Most incorrect codes are due to human error rather than deliberate attempts to cheat. 

If you're missing responses be sure to check the "Responses in Progress" section on Qualtrics. If you have the completion code on the last page of your study and the worker copy and pastes the code and exits the study window without clicking forward in Qualtrics then they'll be listed as a response in progress with e.g. 97% completion. 

---

# Blocks

Blocks are serious business on Mechanical Turk. Amazon has an algorithm which blocks workers from using Mechanical Turk at all if they receive a certain number of blocks (approximately 3 strikes and you're out, though this increases as the number of approved HITs increases). 

It is better to reject their submission and not block the worker. Workers are very aware of rejections because most requesters use a qualification based on the percentage of submissions of approved to screen workers . If you reject their work you don't have to worry about them working for you again (or at least they won't answer randomly again). 

---

# "Soft Block" Qualification - An Alternative to Blocks

Rejecting work should be the first response

If you want to block someone I suggest creating a "Soft Block" qualification and assigning it to workers you don't want participating in your studies. 

Reserve the "hard block" for cheaters or habitually poor and abusvie participants.

---

class: center, middle

# Intermediate MTurking
### Designing Studies for Mechanical Turk
### The Mechanical Turk API 


---

# Important Features for Making Full use of Mechanical Turk

Bonuses - Mechanical Turk gives requesters the ability to pay bonuses to participants. 

Qualifications - Qualifications can allow you to create interesting sub-populations and do multi-part studies. 

API - There is a  Mechanical Turk Requester API which can be used to automate certain tasks and gives access to some options not available through the graphical web requester interface. 
Options for using the API are: Command Line Tools (not recommended), The MTurkR R package, the boto package for Python
* Bonuses and Qualifications can only be granted one at a time through the GUI. To use these effectively requires using the API

---

# Bonuses

This is a great way to run experiments where participants are incentivized. The existing research has shown that MTurkers respond positively to incentives. There are two common ways to gran bonuses: performance based bonuses and bonus lotteries. 

For performance based bonuses a simple way to implement incentives is to give participants different completion codes based on their performance

Bonus lotteries are a good way to increase the stakes of an experiment, and can be combined with performance based incentives by giving lottery tickets based on performance. 

Caveats:
* Make sure that the base pay is still fair if you're using a bonus lottery.
* If bonuses are high and the task lends itself to Googling for an answer don't be surprised if people cheat.
* Some people don't like bonuses if the questions or tasks to get the bonus are too difficult 

---

# Attention & Comprehension Checks

Some research has shown that with the standard quality qualifications on MTurk Attention checks aren't really necessary. 
* If you do use them, be aware that every participant on Mechanical Turk has seen the standard attention checks many, many times

Comprehension Checks
* If you are going to screen out participants on Qualtrics make sure you give them instructions to return the HIT. Do not collect additional data from participants if you're not paying them
* Make sure the comprehension checks are as early as possible, or still collect the survey response and pay participants who fail comprehension checks. 

Because of the nature of Mechanical Turk it is very easy to tell yourself stories about what participants who didn't behave the way you wanted must've been thinking. You should pre-register your analysis plan including exclusions (shout out to Professors Simmons and Simonsohn)

---

# Filtering Out Participants

Common misconception - launching a new batch of a survey will not prevent people who completed the survey in the first batch from retaking the survey

Best Option
* Create a qualification 

Decent Option
* Screen out MTurk IDs in Qualtrics

If you are going to screen out participants on Qualtrics make sure you give them instructions to return the HIT

What Not To Do
* Do *not* block workers to prevent them from retaking a survey. 

---

# Consider Interesting Uses of MTurk 

Consider creative uses of Mechanical Turk instead of viewing it just as an inexpensive way to get high N studies

Example:
Siddharth Suri & Duncan J. Watts - "Cooperation and Contagion in Web-Based, Networked Public Goods Experiments"
Suri and Watts ran 113 experiments where they varied network structure to study cooperation and contagion. This type of research wouldn't be feasible in a lab. 


---

class: center, middle

# Additional Resources and References

---

# Additional Resources

[Amazon Mechanical Turk - Requester UI Guide](http://docs.aws.amazon.com/AWSMechTurk/latest/RequesterUI/Welcome.html)

[Amazon Mechanical Turk - Getting Started Guide for API](http://docs.aws.amazon.com/AWSMechTurk/latest/AWSMechanicalTurkGettingStartedGuide/Welcome.html)

[Turkopticon](https://turkopticon.ucsd.edu/) - Requester Reviews 

[Guidelines for Academic Requesters](http://wiki.wearedynamo.org/index.php/Guidelines_for_Academic_Requesters) - Useful guidelines for being a good academic requester. 

---

# Academic Papers on Mechanical Turk, An Incomplete List 

Berinsky, A. J., Huber, G. A., & Lenz, G. S. (2012). Evaluating online labor markets for experimental research: Amazon. com's Mechanical Turk. Political Analysis, 20(3), 351-368.

Buhrmester, M., Kwang, T., & Gosling, S. D. (2011). Amazon's Mechanical Turk a new source of inexpensive, yet high-quality, data?. Perspectives on psychological science, 6(1), 3-5.

Chandler, J., Mueller, P., & Paolacci, G. (2014). Nonnaïveté among Amazon Mechanical Turk workers: Consequences and solutions for behavioral researchers. Behavior research methods, 46(1), 112-130.

Crump, M. J., McDonnell, J. V., & Gureckis, T. M. (2013). Evaluating Amazon's Mechanical Turk as a tool for experimental behavioral research. PloS one, 8(3), e57410.

Ho, C. J., Slivkins, A., Suri, S., & Vaughan, J. W. (2015, May). Incentivizing high quality crowdwork. In Proceedings of the 24th International Conference on World Wide Web (pp. 419-429). ACM.	

---

# Academic Citations Continued


Ipeirotis, Panagiotis G., Demographics of Mechanical Turk (March 2010). NYU Working Paper No. ;CEDER-10-01. Available at SSRN: http://ssrn.com/abstract=1585030

Mason, W., & Suri, S. (2012). Conducting behavioral research on Amazon’s Mechanical Turk. Behavior Research Methods, 44(1), 1-23. Retrieved from 
http://link.springer.com/article/10.3758%2Fs13428-011-0124-6

Paolacci, G., Chandler, J., & Ipeirotis, P. G. (2010). Running experiments on amazon mechanical turk. Judgment and Decision making, 5(5), 411-419.

Paolacci, G., & Chandler, J. (2014). Inside the turk understanding mechanical turk as a participant pool. Current Directions in Psychological Science, 23(3), 184-188.

Suri, S., & Watts, D. J. (2011). Cooperation and contagion in web-based, networked public goods experiments. PLoS One, 6(3), e16836.
