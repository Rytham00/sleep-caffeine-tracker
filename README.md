# sleep-caffeine-tracker 🌙☕📊
Turning daily habits into data stories ✨

## 📋 Overview
Does caffeine really mess with sleep?  
This project explores daily habits and their impact on sleep patterns using structured CSV logs.

## 📝 Introduction
This project began as an attempt to see whether caffeine alone explained changes in my sleep. Using CSV logs from my habit tracker, I quickly realized caffeine wasn’t the full story. Over time, I expanded the dataset to include wake‑up time and other daily routines to capture a more complete picture of what influences sleep. This repository contains the raw data, analysis scripts, and my findings. It is a personal experiment in turning everyday habits into structured insights.

## 📁 Dataset
- Duration: ~6 weeks of daily logs 📅
- Format: CSV files 📄
- Variables tracked:
  - ☕ Caffeine intake
  - 💤 Sleep hours
  - ⏰ Wake-up time
  - ✅ Exam season 
  - 🌙 Bedtime (planned for future weeks)

## ⚒️ Methodology
- Logged daily habits into a notebook 📓
- Converted notes into structured CSV format
- Analyzed data using Pandas in Google Colab 🐍💻
- Explored correlations with simple statistics and visualizations

## ⚠️ Notes
- Sleep was self reported as approximate ranges and converted to midpoints.
- Variables like 'sleep_time' were read off a hand drawn graph and are accurate to roughly 30 minutes.
- Caffeine amounts were estimated based on typical values per serving.
- Naps were not included, only nighttime sleep.
- Some nights also include long sleep-ins.

## 📊 What I Found
- **Caffeine & sleep:** Caffeine had a weak negative relationship with sleep i.e. higher caffeine days leaned slightly
toward less sleep. However, I also drank more caffeine during exams, so caffeine and exam stress overlap and I can't separate their effects.

- **Exams vs non-exams:** Average sleep was lower during exams but the median was higher. The non-exam average is pulled up by a few very long sleep-ins in October. So "I slept less during exams" is not clearly supported by this data. A fairer description is that my sleep was fairly steady during exams and much more variable afterwards.
  
- **Prediction model:** A simple linear regression using caffeine and exam season did slightly worse than just guessing my average sleep. With this amount of data, caffeine and exam season do not predict my sleep.
  
- **Wake time & bedtime:** Bedtime and wake-up time seem to matter more than caffeine, but I only have about 11 nights of data.

## ⭕ Limitations
- **Small sample:** About 36 usable days, and only 13 of them were exam days. Wake time covers only about 11 nights. A bigger sample size is needed to get proper insights from the data.
    
- **One person:** This is my own data, so the results say nothing about students in general.
  
- **Approximate sleep values:** Sleep hours were read off a hand-drawn graph and are accurate to roughly 30 minutes. Differences smaller than that are not meaningful.
  
- **Estimated caffeine:** Caffeine amounts are estimates based on typical values per serving (for example, per sachet of instant coffee or cup of chai), not measured.
  
- **Overlap with exam season:** Caffeine and stress rose together, so their effects can't be separated. Exam season also includes one revision day before the first paper.
  
- **Missing days:** A few days were not tracked and were left out.
  
- **Naps not recorded:** Sleep time includes only night sleep.
  
- **Long sleep-ins:**  Several 12 to 14 hour nights in October are included as real data and affect the averages. I do not know what caused them.

- **Correlation, not causation:** None of these results show that one thing causes another.
    
## ⌛ Things I plan to do
- Add bedtime tracking
- Add an alarm column
- Re-run at 60+ days
- Expand dataset
 
## 🛠️ Tools I used
- Python
- Pandas
- Scikit-learn
- Google Colab
- I used Claude to help me learn the code and understand the results.
