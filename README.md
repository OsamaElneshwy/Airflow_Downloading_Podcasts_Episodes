# Project Overview
In this project, we'll create a data pipeline using Airflow. The pipeline will download podcast episodes and automatically transcribe them using speech recognition. We'll store our results in a SQLite database that we can easily query.

We don't strictly need to use Airflow to do this project, but it helps us with a few things:

- We can schedule the project to run daily
- Each task can run independently, and we get error logs
- We can easily parallelize tasks and run in the cloud if we want to
- We can extend this project more easily (add speech recognition, summaries, etc) using Airflow
By the end of this project, you'll have a good understanding of how to use Airflow, along with a practical project that you can continue to build on.

🏥 Project DAG Photo 📊
![DAG Overview]([https://github.com/Abdullah28-gheyad/Student-Data-Processor/blob/master/grade_load.png](https://github.com/OsamaElneshwy/Airflow_Downloading_Podcasts_Episodes/blob/main/Project_DAG_Photo.jpeg))

## Project Steps

- Download the podcast metadata xml and parse
- Create a SQLite database to hold podcast metadata
- Download the podcast audio files using requests
- Transcribe the audio files using vosk

## Code
You can find the code for this project here.
File overview:
- podcast_summary.py - the code to create a data pipeline

# Data
We'll download the data we need during this project, including a language model for vosk, and podcast episodes. If you want to view the podcast metadata page, it is here.
