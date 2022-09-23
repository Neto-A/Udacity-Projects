# Udacity-Projects

## Table of Contents.
<ul>
<li><a href="#intro">Introduction</a></li>
<li><a href="#noshow">Project 1: No-Show Appointments 2016</a></li>
<li><a href="#wrangle">Project 2: WeRateDogs- Wrangling and Analysing.</a></li>
</ul>

<a id='intro'></a>
## Introduction.
This is a repository containing my submitted and approved technical projects for my Udacity Data Analyst Nanodegree course. There are 2 projects included here, with one more still in the works.

<a id='noshow'></a>
## Project 1: No-Show Appointments 2016

### Dataset Description 

This is my first technical project for the nanodegree course. I cleaned, analyzed and visualized the No-Show Appointments dataset, obtained from [Kaggle](https://www.kaggle.com/datasets/joniarroba/noshowappointments?page=3). 
The dataset contained over 100,000 entries, arranged over the following columns:
   * PatientId: Each patient's unique identification number.
   * AppointmentID: Each patient's unique identification number for each scheduled appointment.
   * Gender: Female (F) or Male (M)
   * ScheduledDay: The date and time each appointment was scheduled.
   * AppointmentDay: The actual date of each scheduled appointment.
   * Age: Patients' ages.
   * Neighbourhood: where each patient lives
   * Scholarship: whether or not the patient is enrolled in [Bolsa Família](https://en.wikipedia.org/wiki/Bolsa_Fam%C3%ADlia), a welfare program set up by the Government of Brazil, between 2003 and 2021.
   * Hipertension: records of whether each patient has hypertension or not.
   * Diabetes: records of whether each patient has diabetes or not.
   * Alcoholism: records of whether each patient suffers from chronic alcoholism or not.
   * Handcap: records of whether each patient has some sort of handicap or not.
   * SMS_received: records of whether each patient received an SMS reminder for their scheduled appointment or not.
   * No-Show: records of whether or not a patient met an appointment. Here, 'No' means the patient was not a no show, i.e. the patient kept the appointment.

   *For all the records from Scholarship to SMS_received, 1 means positive (or received) or negative (or not received).*


### Questions for Analysis
>At a glance, before getting into the rest of the process, I posed a few questions to be answered at the end of this analysis. These questions guided further wrangling and analysis of the data.

   1. What percentage of patients __kept__ their scheduled appointments?
   2. Which gender is more likely to __schedule__ an appointment?
   3. Patients of which age groups are most and least likely to __schedule__ an appointment? Least likely?
       * These questions reflect on [health seeking behaviour](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6143883/#:~:text=Healthcare%20seeking%20behaviour%20(HSB)%20has,behaviour%20or%20sick%2Dterm%20behaviour) of patients.     
   4. Which gender is more likely to __keep__ an appointment?
   5. Patients of which age groups are most and least likely to __keep__ an appointment? 
   6. From what neighbourhood do the most patients who keep their appointments come? 
   7. From what neighbourhood do the fewest patients who keep their appointments come? 
   8. How many patients on Bolsa Familia keep their appointments?
   9. Do certain conditions (in this case, hypertension, diabetes, alcoholism and handicap) affect showing up for appointments?
   10. Does receiving an SMS reminder help patients keep their appointments?
   
<a id='wrangle'></a>
## Project 2: WeRateDogs- Wrangling and Analysing.
This was my second technical project for the nanodegree course. This project specifically targets data wrangling skills. I scraped tweets from WeRateDogs' (@dog_rates) Twitter archive, using the Tweepy API. I then visually and programatically assessed, cleaned and analyzed the data.  

### Dataset Description.
- tweet_id: The last part of the tweet URL after "status/"
- date_created: The date and time each tweet was posted.
- source: The type of device the tweet was made from.
- text: The full content of the tweet.
- expanded_url: The link to each tweet.
- rating_numerator: What each dog was rated out of (mostly) 10.
- name: The name of each rated dog.
- dog_stage: Whether each dog is a doggo, floofer, pupper, puppo or none. Explanations for these groupings are contained in this [dogtionary](https://video.udacity-data.com/topher/2017/October/59e04ceb_dogtionary-combined/dogtionary-combined.png).
- favorite_count: Number of 'likes' each tweet garnered.
- retweet_count: Number of 'retweets' each tweet garnered.
- jpg_url: Link to each image contained in each tweet.
- p1: the algorithm's #1 prediction for the image in the tweet
- p1_conf: how confident the algorithm is in its #1 prediction 
- p1_dog: whether or not the #1 prediction is a breed of dog 
- p2: the algorithm's second most likely prediction
- p2_conf: how confident the algorithm is in its #2 prediction
- p2_dog: whether or not the #2 prediction is a breed of dog
- p3: the algorithm's third most likely prediction
- p3_conf: how confident the algorithm is in its #3 prediction
- p3_dog: whether or not the #3 prediction is a breed of dog

### Questions for Analysis.

At a glance, before getting into the rest of the process, I posed a few questions to be answered at the end of this analysis. These questions guided further wrangling and analysis of the data.
1. What are the top 3 dog stages by frequency?
2. What are the most liked tweets?
3. What are the most retweeted tweets?
4. What is the average level of confidence of the algorithm in its image predictions?
5. Is the prime prediction a dog species?
