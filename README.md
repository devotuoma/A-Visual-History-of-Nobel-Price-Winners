A Visual History of Nobel Prize Winners (1901–2016)

<img width="1082" height="321" alt="Screenshot 2025-11-20 at 11 37 58" src="https://github.com/user-attachments/assets/3f151908-3145-4f56-b5df-acb0d71313ba" />


I’ve always been fascinated by how big, prestigious awards like the Nobel Prize evolve over time — who gets recognized, which countries dominate, and how things like gender and age representation shift throughout history. So I decided to dig into the full dataset of Nobel Prize winners from 1901 to 2016 and see what stories the numbers would tell.

 GitHub Repo:
https://github.com/devotuoma/A-Visual-History-of-Nobel-Price-Winners


This project became a mix of data cleaning, exploration, and a lot of visualizations to make sense of more than a century’s worth of award history.

 What I Set Out to Do
 

My goal wasn’t just to crunch numbers — I wanted to understand the bigger picture:

Which countries have historically dominated the Nobel Prizes?

When did the U.S. take over as the top producer of laureates?

How badly skewed is gender representation, and has it improved?

How old are Nobel Prize winners, really — and has that changed?

And who are those rare people (or organizations) who won more than once?

The dataset from the Nobel Foundation includes a ton of useful information: names, categories, birth countries, genders, birth dates, and award years — basically everything you’d want to run a demographic time-travel analysis.


 
 Getting the Data in Shape

I loaded up Pandas, NumPy, Seaborn, and Matplotlib and pulled the dataset in:

import pandas as pd
import numpy as np
import seaborn as sns

nobel = pd.read_csv('datasets/nobel.csv')


From there, I cleaned up the date columns, fixed inconsistent country labels, and created new variables like whether a laureate was U.S.-born and their age at the time of receiving the award.


 What I Found
1️ Country Dominance Isn’t Static

In the early decades, Europe — especially the UK, Germany, and France — completely dominated.

But then things shifted.


2️ The Rise of the United States
<img width="707" height="570" alt="Screenshot 2025-11-20 at 12 15 44" src="https://github.com/user-attachments/assets/8ddeb543-e476-4c18-a5c7-2a36e9f31ad9" />


By tagging U.S.-born winners and plotting them by decade, the story became clear:

The U.S. starts pulling ahead in the 1930s and hasn’t looked back since.

This lines up with major scientific investment in the U.S. around that time, especially pre- and post-WWII.



3️ Gender Imbalance Is… Severe
<img width="980" height="647" alt="Screenshot 2025-11-20 at 12 16 50" src="https://github.com/user-attachments/assets/3d987d98-53be-4816-98b5-b2ce0d084cf5" />


No surprises here, but seeing the numbers laid out decade by decade makes it even more striking.

For a long time, female laureates were extremely rare.

Things improve (slowly) in recent decades.

Peace and Literature show the most progress.

Physics and Economics? Still overwhelmingly male.


4️ The First Woman: Marie Curie


It was nice to confirm that the very first female Nobel Prize winner was indeed Marie Curie in 1903 (Physics), and she later won another one in Chemistry.

She’s also one of the very few people ever to win twice.


5️ Repeat Laureates Are Almost Mythical

Only a tiny group has won multiple Nobel Prizes, among them:

Marie Curie

John Bardeen

Linus Pauling

Frederick Sanger

The Red Cross & UNHCR

Most people never win one — winning two puts you in superhero territory.


6️ Age Patterns Are Changing
<img width="1343" height="610" alt="Screenshot 2025-11-20 at 12 17 42" src="https://github.com/user-attachments/assets/7516b26a-5761-4af9-810c-6b5fd7e9c5d6" />
<img width="679" height="371" alt="Screenshot 2025-11-20 at 12 19 47" src="https://github.com/user-attachments/assets/9493dec6-4915-4d11-8ced-70f92974ced3" />
<img width="681" height="339" alt="Screenshot 2025-11-20 at 12 21 04" src="https://github.com/user-attachments/assets/63213407-91b5-43aa-b3cc-7a21f0969301" />
<img width="683" height="340" alt="Screenshot 2025-11-20 at 12 21 16" src="https://github.com/user-attachments/assets/6472b1d0-1b98-47a6-b295-68c5add3aeb5" />
<img width="684" height="343" alt="Screenshot 2025-11-20 at 12 21 27" src="https://github.com/user-attachments/assets/7ea81c51-d721-42aa-8fd9-2868ef3d422f" />
<img width="682" height="337" alt="Screenshot 2025-11-20 at 12 21 37" src="https://github.com/user-attachments/assets/44bb81c5-d072-4687-84a0-1a79a693107e" />
<img width="681" height="340" alt="Screenshot 2025-11-20 at 12 21 48" src="https://github.com/user-attachments/assets/b25d405f-b17b-4664-bf1e-2ec104e3a9e3" />




By calculating age at the time of award, I noticed:

Early laureates were often in their early 50s.

Modern laureates are closer to their mid-60s.

Physics has the strongest trend toward older winners (maybe because cutting-edge breakthroughs take longer now?).

The Peace Prize is the opposite — it has gotten younger in recent years.



7️ Youngest & Oldest

Youngest ever: Malala Yousafzai (17)

Oldest ever: Leonid Hurwicz (90)

The age spread is pretty wild.

 Bringing It to Life with Visuals

I plotted everything from U.S. dominance to gender proportions to age regressions across categories. Visuals made the century-long patterns much easier to spot and understand.


 
 Tools I Used

Python for everything

Pandas for data wrangling

NumPy for numerical work

Seaborn + Matplotlib for charts




 
 What I Took Away

The global center of scientific and cultural influence really did shift to the U.S. in the 20th century.

Gender imbalance in Nobel Prizes is not only real — it’s massive.

Laureates are getting older, likely because modern research and discovery take longer.

Only a few people have achieved multiple Nobel wins, which shows how rare that kind of recognition is.


 
 Want to Try It Yourself?
git clone https://github.com/devotuoma/A-Visual-History-of-Nobel-Price-Winners
pip install pandas numpy matplotlib seaborn


Open the notebook in Jupyter or VSCode and you’re good to go.
