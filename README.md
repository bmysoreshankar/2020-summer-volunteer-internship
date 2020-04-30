# Read this first
If you decide to help support non-profits by working on Opportunity Hack this summer, you need to be made aware of a few things.

0. Opportunity Hack is run by volunteers who have full-time jobs.  We'll be making time to help you this summer.
1. This is the first time we're doing this.
2. We're doing this to provide experience and education over the summer for students who may have had difficulty in finding internships, either because they couldn't find one or because it was [cancelled](https://github.com/gcreddy42/hiring2020).
3. There is no guarentee that you'll receive a job from the work you do with this internship.
4. All of the work you do will be publically available (i.e. Slack, GitHub, demos will be recorded and published on YouTube) for any employer and for you to put in your portfolio.  Ideally the effort you put in is equal to your chances for success in the future.
5. We cannot offer official letters of employement (if you are on a visa) as we are a group of people who volunteer our technology-focused minds to help non-profits.  You'd be joining us in our guild.  Hopefully by the same time next year we'll have an official non-profit and we can help with letters of employement.  This is not an unpaid internship, this is you volunteering your time over the summer.


# Table of contents
1. [Outcomes](#outcomes)
2. [Projects](#projects)
3. [Schedule](#schedule)


# Outcomes
## Your benefit
By working on an Opportunity Hack project over the summer, you'll not only be helping your community, but you'll learn these skills:
1. Learn GitHub
2. Agile - sprints, demos, planning
3. Write code
4. Work with a team

Some other things:
1. Public proof of your work for your portfolio
2. A document that describes the work you put in this summer
3. A recommendation for above-and-beyond effort

## Our benefit
1. We'd love to prove that a virtual summer project can work
2. Continued work on meaningful projects we have identified for non-profits
3. Making connections with you

# Projects
These projects come from our years of experince working with non-profits, we sought to generalize the problems we see in order to impact many non-profits, so although you'll see a few called out, we intend for these solutions to be used at scale, globally, at a relatively inexpensive price point.


## 1. Digitize Paper Forms
Slack Channel: `#2020-vol-intern-digitize-paper-forms`

Non-profits are using paper forms.  The cost to digitize these forms to an HTML form in order to integrate it into their existing systems is difficult.  Google Forms is great, yes, but it still requires some effort and knowledge without allowing integration with existing software applications.  We have been working with ASU on two senior capstones around this problem that we can leverage as a head start.

### Requirements
1. You'll be given an [YOLOv3](https://pjreddie.com/darknet/yolo/) ML model (from our work with ASU)
2. You'll be given two images of paper forms
3. Given the bounding boxes output from the ML model, the solution shall create an HTML-based form for each image
4. The solution shall handle additional images in the future
5. The solution shall store the data submitted in the form
6. The solution shall be deployable via 1-button click with a service like [Heroku](https://www.heroku.com/)
### References
- 2018 Proposal for ASU Tempe [Digitize Paper Forms with Machine Learning Part 1](https://docs.google.com/document/d/1xZSuvGs2s-AP4staL0lyeUUDJCBc_DggPglEpLoMZI8/edit?usp=sharing)
- 2019 Proposal for ASU Tempe [Digitize Paper Forms with Machine Learning Part 2](https://docs.google.com/document/d/1nXNlYUaABAfAKbmi1ZnU79VgFa7B5NLPTkdw4dxIRVU/edit?usp=sharing)
- [Mi Benefial Legal](https://github.com/opportunity-hack/Arizona/issues/46) problem statement history from Opportunity Hack
- [National Kidney Foundation](https://github.com/opportunity-hack/Arizona/issues/24) problem statement history from Opportunity Hack
- [2019-2020 ASU Capstone Github Repo](https://github.com/MrPanda1/YOLO-FormDataset)
- [2018-2019 ASU Capstone GitHub Repo](https://github.com/opportunity-hack/digitize-paper-forms)


## 2. Simple Electronic Healthcare Records (EHR)
Slack Channel: `#2020-vol-intern-simple-ehr`

Some non-profits have "clients" that require demographics and treatment to be tracked easily.  This usually requires some scheduling component as well as a historical record of visits with services provided, then reports follow.  There are open-source EHR solutions on the internet, but none are simple enough for non-profits to use without dedicated training.
### Requirements
1. The solution shall allow for clients to register for the system, using Google Single Sign-on or system-based account creation
2. The solution shall record "treatments": medicine provided, music session, painting
3. The solution shall allow for role-based access: 
4. The solution shall log an audit record of activity
5. The solution shall be secure: (1) no security violations for packages, (2) strong authentication
6. The solution shall use an existing framework (e.g. [Django](https://hackernoon.com/configure-role-based-access-control-in-django-74fa94a54aff)) that offers authentication and role-based access.
7. The solution shall allow for data to be import via CSV including patient records and schedule
8. The solution shall be deployable via 1-button click with a service like [Heroku](https://www.heroku.com/)
### References
- [Chandler CARE Center](https://github.com/opportunity-hack/Arizona/issues/44) problem statement history from Opportunity Hack
- [Neurologic Music Therapy Services of Arizona (NMTSA)](https://github.com/opportunity-hack/Arizona/issues/31) problem statement history from Opportunity Hack
- [2nd Place Opportunity Hack 2019 project](https://devpost.com/software/chandler-care-center-data-intake) for Chandler CARE Center
- [Opportunity Hack 2017 project for NMTSA](https://devpost.com/software/team-3-nmtsa)
- [Opportunity Hack 2019 project for NMTSA](https://devpost.com/software/nmtsa-scheduleapp)

## 3. Risk Scoring
Slack Channel: `#2020-vol-intern-risk-scoring`

Non-profits need a way to vet the standing of people, specifically for pets, as they want to be sure they are going to a nice home.  Given a social media profile (and potentially their network) that someone has granted access to, analyze the content of their posts to create a risk score to understand if there are any red flags for pet adoption.
### Requirements
1. The solution shall collect posts and bio information from Facebook or Twitter
2. The solution shall provide a high risk score for accounts that use terms that indicate violence, hate, animal cruelty, and malice -  this likely means that you will be looking for accounts that already exhibit this, or you can create mock accounts to validate and test the scoring methodology
3. The solution shall be deployable via 1-button click with a service like [Heroku](https://www.heroku.com/)
4. The solution shall provide a URL that a non-profit can send to a potential animal adopter.  This potential animal adopter will use this URL to sign into either Facebook and Twitter to allow this application to collect data as stated above in order to collect data that may not be publically available per privacy settings the user has provided
5. The solution shall not store data from the person's Facebook or Twitter account that is not private
6. The solution shall store the risk score along with the URL that was provided to the potential animal adopter
### References
- [Saving One Life Animal Rescue and Sanctuary](https://github.com/opportunity-hack/Arizona/issues/43) problem statement history from Opportunity Hack
- [My First Machine Learning Project: Designing a Hate Speech Detecting Algorithm](https://towardsdatascience.com/my-first-machine-learning-project-designing-a-hate-speech-detecting-algorithm-56ab32f10833)
- [Hate Speech Detection Using Natural
Language Processing Techniques](https://science.vu.nl/en/Images/werkstuk-biere_tcm296-893877.pdf)


## 4. Data Analysis
_Still working on these details_

Slack Channel: `#2020-vol-intern-data-analysis`

### 4.1 Analyze trends to recommend areas of focus
- https://github.com/opportunity-hack/Arizona/issues/36

### 4.2 Allow non-profits to print forms, collect responses, scan them and easily analyze the data
- Productionalize [Survey Stack](https://devpost.com/software/survey-stack) from Opportunity Hack 2018 for [Animals and Humans in Disaster Inc.](https://github.com/opportunity-hack/Arizona/issues/35), [RealTimeSTEAM](https://github.com/opportunity-hack/Arizona/issues/36), and [NMTSA](https://github.com/opportunity-hack/Arizona/issues/31).



## 5. Volunteer registration and tracking
There are a ton of non-profits that want to allow volunteers to register on their website, 
_Still working on these details_

Slack Channel: `#2020-vol-intern-volunteer-registration-and-tracking`

Perform market research to recommend a system for all non-profts to use.
### Requirements
1. Be able to list times available for volunteers along with location and duration of request
2. Be able to specify skill that is needed (e.g. painting, drywall, electrical, math tutor, etc.)
3. Increase communication between NPO and volunteers to increase engagement
4. Be able to find volunteer opportunities in a region
5. Be able to find opportunities that are good for families
6. Recommend volunteer opportunities based on previous experience
## References
- SignupGenius 


## 6. Intelligent Donation Platform
_Still working on these details_

Increase recurring donations or volume of donations
### Requirements
1. Recommend other items to donate: if someone donates a TV, ask if they also have shoes to donate
2. Cluster similar donors together to determine alternative marketing methods that may be more effective within the cohort


## 7. Inventory management system
_Still working on these details_


## 8. Notification system
_Still working on these details_



# Schedule
## Full Schedule
- Group A: May 8th to July 3rd
- Group B: May 22nd to July 17th
- Group C: June 12th to August 7th

## Agile meetings
- Standups: Every Monday and Wednesday (via Slack).  
- Demo meetings: Every 2 weeks on Friday - recorded and published to YouTube
- Planning meetings: Every 2 weeks on Wednesday

## Mentor "office hours"
- Every week to start for the first 2 weeks
- Switch to 2-week meetings after first 2 weeks
