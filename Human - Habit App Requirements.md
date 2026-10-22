#habitapp

Goal: I need a habits app to display on my life dashboard. I am currently using Habit Pixel, which has the following UI card for a single habit: 

![[Pasted image 20261021190124.png]]

# User Interface
1. A card similar in style to what Habit Pixel uses, pictured above
2. The block calendar showing completion history for the goal, with the week starting on Monday
3. A unique, bright color for each habit
4. Streak indicator (the number next to the fire icon)

# Streaks
A streak is a count of how many days a habit has been completed according to the set goal in a row. A streak should count up by one per day until it is impossible for the goal to be met. If the user backdates habit completions, the streak should be updated to match. If a goal frequency is changed, we maintain the streak even if the new goal wasn't met in the past. 

# Configuration
This info is required when a new habit is created. 
1. Habit title
2. Goal frequency (e.g. "3x per week", "every day", etc.). This needs to also take into account multiple goal completions per day (e.g. "do y 5 times a day every day"). It also must take into account specific days of the week (e.g. "do y on Monday, Wednesday, and Friday every week"). 
Example Configuration UI for 3x per week:
![[Pasted image 20261021185644.png]]

