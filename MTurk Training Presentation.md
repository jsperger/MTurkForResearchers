# What is Mechanical Turk (MTurk)?

Mechanical Turk is an online crowd sourcing platform created by Amazon. The site acts like a job board - Requesters can post jobs (Human Intelligence Tasks in MTurk parlance) which can be completed by Workers. 


Mechanical Turk is very popular with researchers in psychology because you can quickly collect survey responses for a low cost. Two of the most common use cases are pilot testing studies and study components and running high powered studies. The typical MTurk study is generally shorter and less complex than a lab study (though not necessarily true). 

---

# What does research say about Mechanical Turk as a participant pool?

The Good
* Inexpensive source of high quality data. Mechanical Turk Participants seem to be at least as attentive as lab participants. 
* Papers with studies run on Mechanical Turk are widely accepted
* Workers want to do a good job 
 *  This past spring someone in the departmetn ran an experiment where participants were paid up front for a two part study. 
 
The Concerns
* There is cross-talk between participants
 * Usually don't reveal manipulations, the discussion is more about what studies are high paying and which requesters are good. However if you have a manipulation that would be considered annoying participants might discuss it with each other. 
* Professional Participant Pool
 * This isn't really different from lab studies 

---

# Creating a New HIT

![Create New Project](/Images/Create\ New\ Project.png)

---

# New Project - Survey Link

![New Project - Survey Link](/Images/New\ Project\ Survey\ Link.png)

---

# Components of a HIT - Description

![Mturk Hit Description Example](/Images/"HIT Description".png)

* Title - The title alone is what workers first see when looking for HITs; sentences instead of single words are the standard
 * Typically you should include the estimated time to complete in the title of the HIT
* Description - Give more detail about the task. 
 * If your HIT contains the following you should mention it explicitly in the description: writing tasks, video watching, listening to audio
* Keywords - keywords that workers can use to search for your HIT

---

# A Brief Note on Time Estimates

Providing accurate time estimates is one of the most important things you can do as a requester. 

* The average worker on Mechanical Turk probably reads more slowly than you
* Keep in mind that you've seen your study materials before. Even if you try to read carefully you'll probably still end up skimming if you try to estimate the completion time for your own study. 

For short studies try to avoid giving a range of times. A "1-3 Minute Study" which pays fifteen cents could correspond to hourly wages of $9.00/hr, $4.50/hr, or $3.00/hr.

Rule of Thumb: If a study is five minutes or less don't give a range. 

---

# Components of a HIT - The Set Up

![HIT Set Up](/Images/HIT\ Set\ Up.png)
* Reward per assignment
 * MTurk standard is 10 cents/minute which works out to $6.00/hour
 * We should do better - The federal minimum wage is $7.25/hour
 
* Number of assignments per HIT 
* Time alloted per assignment - this is *not* how long your HIT takes to complete. This is how long a worker has to complete the HIT before Amazon automatically prevents the worker from submitting the HIT and allows another worker to have a chance to complete the assignment. 

---

# Components of a HIT - Worker Requirements

![Worker Requirements](/Images/Worker\ Requirements.png)

* Master Workers - costs extra money and is basically useless provided you use sensible worker qualifications

* Standard qualifications - 95% approval, Greater than 100 HITs Approved, Location is United States

---

# Additional Qualifications


---

# Designing Studies for Mechanical Turk


---

# Options for Confirmation

Payment Code

External Question 

---

# Bonuses

If bonuses are high and the task lends itself to Googling for an answer don't be surprised if people cheat.

---

# Attention Checks

* Every participant on Mechanical Turk has seen the standard attention checks many, many times

Comprehension Checks

 *Pre-register your analysis plan (shout out to Professors Simmons and Simonsohn)

---

# Filtering Out Participants

Common misconception - launching a new batch of a survey will not prevent people who completed the survey in the first batch from retaking the survey

Best Option
* Create a qualification 

Decent Option
* Screen out MTurk IDs in Qualtrics

If you are going to 

Do Not Do
* Do not block workers to prevent them from retaking a survey. 

---

# A Note on Blocks

Blocks are serious business on Mechanical Turk. Amazon has an algorithm which blocks workers from using Mechanical Turk at all if they receive a certain number of blocks (approximately 3 strikes and you're out, though this increases as the number of approved HITs increases). 

From a worker's perspective it is better to have a submission rejected than it is to have the submission accepted but then blocking them. 
For example: Imagine you have a survey and a participant seems to have responded randomly. You might think "Well, they arguably completed the survey but I don't want them completing any surveys in the future for me" and want to accept their submission but block them.

It is better to reject their submission and not block the worker. Workers are very aware of rejections because most requesters use a qualification based on the percentage of submissions of approved to screen workers . If you reject their work you don't have to worry about them working for you again (or at least they won't answer randomly again). 

---

# "Soft Block" Qualification - A Blocking Alternative

If you really want to block someone I suggest creating a "Soft Block" qualification and assigning it to workers you don't want participating in your studies. 

Reserve the "hard block" for repeat offenders and cheaters.

---

# Requester Best Practices

Pay well

Approve Work Promptly

Don't be a jerk

If it looks like a lot of people are cheating, you probably screwed up. In the past year of running the department's account I have collected ~150,000 survey responses. In that time I've had to block only three people for deliberate attempts to cheat. 
Most incorrect codes are due to human error rather than deliberate attempts to cheat. 

---

# Not all participants are nice

If you reject someone's work they will sometimes send you nasty emails. 

While purely anecdotal evidence, I've noticed that some of the workers who submit the worst work will most aggressively message you to try to shame you into reversing the rejection. 

---

# Amazon Terms of Service

* You can't collect Personally Identifying Information (PII) - this includes email addresses. 

* If your survey contains adult content it must be flagged. 

---

# Advanced Mechanical Turk

* The Mechanical Turk Requester API
 * Command Line Tools
 * The MTurkR R package
 * The boto package for Python
 
---

# Additional Resources

[Amazon Mechanical Turk - Requester UI Guide](http://docs.aws.amazon.com/AWSMechTurk/latest/RequesterUI/Welcome.html)

[Amazon Mechanical Turk - Getting Started Guide for API](http://docs.aws.amazon.com/AWSMechTurk/latest/AWSMechanicalTurkGettingStartedGuide/Welcome.html)

[Turkopticon](https://turkopticon.ucsd.edu/)

[Guidelines for Academic Requesters](http://wiki.wearedynamo.org/index.php/Guidelines_for_Academic_Requesters) - Useful guidelines for being a good academic requester. 

---

# Academic Papers on Mechanical Turk

Mason, W., & Suri, S. (2012). Conducting behavioral research on Amazon’s Mechanical Turk. Behavior Research Methods, 44(1), 1-23. Retrieved from http://www.ncbi.nlm.nih.gov/pubmed/21717266\nhttp://www.springerlink.com/index/10.3758/s13428-011-0124-6

