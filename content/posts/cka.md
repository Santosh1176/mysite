---
author:
  name: "Santosh Kaluskar"
date: "2023-03-22"
linktitle: "Cracking the CKA Exam: Insights and Tips from a Successful Candidate"
type:
- post
- posts
title: "Cracking the CKA Exam: Insights and Tips from a Successful Candidate"
weight: 10
series:
- Experience
---

The Certified Kubernetes Administrator (CKA) certification is a globally recognized certification for professionals who want to demonstrate their expertise in managing and administering Kubernetes clusters. It is a performance-based examination that checks for candidates' competency in the following area:

- Understanding Kubernetes core concepts such as Pods, Deployments, Service, Authentication, Authorization, Kubernetes Networking Model, etc.
- Tests the candidate's ability in deploying and managing Kubernetes.
- Skills required for troubleshooting and debugging issues in a Kubernetes cluster
- Understanding of Kubernetes Security primitives and best practices to be followed in a Kubernetes environment by securing workloads deployed on a cluster and by protecting sensitive data.

I recently took the exam and cleared it on the first attempt. It was a great journey. When I got my CKA certificate from the Linux Foundation, which realized all the hard work put in not only by me but by all the people who enabled me to learn all the relevant topics of such a complex technology — Kubernetes. especially Mumshad Mannanbeth from KodeKloud, all the community coaches from the KodeKloud community, and many others.

In this post, I will share my experiences of learning about Administrating Kubernetes clusters and some tips that could help fellow CKA aspirants clear the exam on the first attempt.
Below are some of the pointers that I would like to share with fellow CKA aspirants:

## Make it a habit of referring to official documents, as that would be your closest aid during the exam. This is one of the most important things I've learned.

I assure you, apart from hands-on experience gained from the KodeKloud or any other course for that matter. The only thing you need to refer to and get accustomed to is the Kubernetes official documents. This is one source we are allowed to refer to during the exam and we need to be quite comfortable finding the right resource using the docs' search functionality.

## Practice Active Recall — Always take a short break and attempt the labs again.

This is the choice I made, many people may differ with me here. I chose to practice [Active Recall](https://aliabdaal.com/activerecallstudytechnique/) while preparing for the exam. This helped me in strengthening the lessons learned and better understand the topics.

## Practice working with imperative commands and generate yaml using --dry-run=client -o yaml flags as much as you can.

I practiced a lot using imperative commands to create objects. I assure you this skill will be a great time saver during the exam. Along with this, I would also suggest using the `--help` command liberally while creating any Kubernetes object.

## Learn and practice JSONPath query language.

We will be working a lot with `yaml` files and as we know YAML is a superset of JSON. [JSONPath is a query language](https://santoshdts.hashnode.dev/working-with-json-data-with-jsonpath-a-beginners-guide) when applied to a given JSON dataset gets you results that are subsets of the given dataset. We can apply JSONPATH queries to our YAML dataset to get desired values of a specific field in the YAML structure. You can learn more about jsonpath and practice it with the hands-on labs on [KodeKloud's free course](https://kodekloud.com/courses/json-path-quiz/).

## Practice debugging containers a lot  with `crictl`

Post depreciation of Docker as CRI for Kubernetes. `crictl` is the defacto to [inspect and debug container runtimes and applications on a Kubernetes node](https://kubernetes.io/docs/tasks/debug/debug-cluster/crictl/). Try practicing with `crictl` as much as possible. As we might be dealing with tasks where the pods can go down for a brief period of time. This is where we need to turn our attention and focus on Containers and their status. this is practicing with `crictl` comes in handy.

## Practice the Lightning labs and Mock exams until you can complete the exams with a 100 score within 20-30 mins

I can't stress more about KodeKloud's Lightning Labs and Mock exams. I literally retook the Lightning Labs and Mock exams multiple times until I felt comfortable and was able to complete each exam within 20-30 mins with a 100% score. That gave me a lot of confidence.

## Precursor to the real CKA exam, the Killer.sh sessions
The claim Killer.sh makes is not false, it was a bit harder coming from completing the same tasks in the KodeKloud Mock exams within 30 mins. I was able to attempt only about 16 questions on my first attempt and scored 72 out of 125. The experience of the killer.sh exam environment closely resembles the exam environment of the real CKA exam. This really helped me get a first-hand experience of how the real exam environment would be. Here, I identified some more complex knowledge gaps I had and went back to lectures, labs, and official docs.

The above points I mentioned are quite obvious to everyone planning to attempt the CKA exam. But what followed after completing my first killer session is the one which I need to share with you. This is where I struggled a lot and could not achieve my full potential.

## I'd caution my fellow CKA candidates to stay away from the following:


Scheduling is one of the most important aspects that a candidate should be aware of. The Linux Foundation provides us with the [checklist](https://docs.linuxfoundation.org/tc-docs/certification/quick-guide/schedule-an-exam) once we purchase the exam that we need to complete. 

![cka-checklist](https://user-images.githubusercontent.com/91916466/226903661-7cc7423f-bc1e-4903-bb6f-fd3ead7b2e60.png)

I feel this contains some important documents, namely, The Candidate Handbook and Important Instructions. These documents I believe are of equal importance as compared to the subjects in the curriculum. **I advise every candidate should through these documents multiple times at least and especially read them thoroughly once just before appearing for the exam.** It contains all the details that a candidate should know about the exam environment, all the dos and dont's, etc, and answers most of the questions a candidate is having in his mind. **I went through the document the very first time just a few days before the exam. It was one of my Biggest Mistakes**. However, unaware of the consequences I went ahead and scheduled the exam. As I had to take the exam from my home and the exam requirement is of having a quiet surroundings. I was provided with the choice of 0200 hrs and 0300 hrs IST. I chose the earlier one. I advise you to Schedule your exam according to your comfortable timings and be sufficiently rested before your exam day.


I activated my second killer session after a break of learning all the topics for a period of 10 days and **just 2 days before the CKA exam**. In this second session, I was again able to score 100-110 within two hours. I practiced the mock exams for their full-time period i.e. 36 hours without wasting any time. My thought process was like, I would be fully prepared if I do not have much time gap between the last killer session and the real exam. But I was wrong!

## The Big Day

As I had recently completed my second killer session hours before the exam day and felt very confident and high on morale. But, I was very exhausted due to working on the killer.sh session AND I had scheduled the exam at the odd hour of 2 AM IST. The pre-exam procedures were completed very smoothly for me, which I was very much worried about from reading about some of the bad experiences of fellow candidates. Then I was presented with the EXAM.

- **Go through the Candidate Handbook multiple times and at least once before the exam**
After purchasing the Exam, the very first thing I would advise is of downloading a Copy of the Candidate Handbook and Important instructions on your Laptop and on your mobile as well. Whenever you have any doubts regarding the exam, this should be your first and the best place where you will find answers to your queries regarding exam.

- **Please, Please, Go through the walkthrough guide of the exam environment which is provided immediately after producing the Exam to You. [The actual exam timer will start after you hide the tour button or the tour ends](https://docs.linuxfoundation.org/tc-docs/certification/lf-handbook2/exam-user-interface/examui-performance-based-exams#guidelines-and-tips-for-using-the-remote-desktop)**
This is where I did yet another mistake by closing the guided tour and heading directly to the exam tasks. I was confused throughout the exam. More than the exam environment, it was the mistake I did which was lingering in my mind throughout, which took a toll on my performance.   

- **Go through the question slowly and clearly and understand the requirement**
Hurring-up will surely not help you in any way. In fact, trying to speed up the initial process of understanding the requirements of the task may hamper the final outcome. Take it easy and read through the questions clearly. 

- **Use the MousePad app for taking notes, like uncompleted tasks, tasks which you need to return back, etc** 
This is Yet another blunder I committed during my exam. Every candidate has their own strategy to deal with exam questions, the one I follow and would recommend to others is to tackle the low-scoring and relatively easy tasks first and head over to high-scoring and complex tasks. For this, you need a tool to keep track of the questions you've completed, partially completed, and questions that you would like to revisit after completing the easy one. The inbuilt MousePad note-taking app is made for that purpose, Due to my earlier mistakes lingering in my mind, I totally forgot to keep track of the status of the questions. 

- **Always keep a backup of the object which you intend to work on**
There are chances, the work you have carried out on some object might work out as intended and consequently the Kubernetes object or sometimes the cluster might not come up. In such cases we can fall back on the backup we had taken earlier. That would save you from some serious headaches. 

- **Always verify the work you have done in order to accomplish the given task.**
We might assume and be confident about the process that we have implemented. But, there are possibilities that we might have missed an important but subtle nuance in the question that might have skipped our eyes. To avoid such complications, it's always better to cross-check and re-confirm the desired outcome of the task.



# Conclusion

Overall the exam was a great experience and I learned a lot in the process. With all the training at KodeKloud and investing some time and enough practice, clearing the CKA should not be a tough nut to crack. But I would advise considering some of my experiences that would make your CKA journey pleasant and memorable. I hope my experiences would be helpful to many and feel free to share your questions, comments, and feedback.