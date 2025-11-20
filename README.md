📊 A Visual History of Nobel Prize Winners (1901–2016)

I’ve always been fascinated by how big, prestigious awards like the Nobel Prize evolve over time — who gets recognized, which countries dominate, and how things like gender and age representation shift throughout history. So I decided to dig into the full dataset of Nobel Prize winners from 1901 to 2016 and see what stories the numbers would tell.

🔗 GitHub Repo:
https://github.com/devotuoma/A-Visual-History-of-Nobel-Price-Winners

This project became a mix of data cleaning, exploration, and a lot of visualizations to make sense of more than a century’s worth of award history.

📝 What I Set Out to Do

My goal wasn’t just to crunch numbers — I wanted to understand the bigger picture:

Which countries have historically dominated the Nobel Prizes?

When did the U.S. take over as the top producer of laureates?

How badly skewed is gender representation, and has it improved?

How old are Nobel Prize winners, really — and has that changed?

And who are those rare people (or organizations) who won more than once?

The dataset from the Nobel Foundation includes a ton of useful information: names, categories, birth countries, genders, birth dates, and award years — basically everything you’d want to run a demographic time-travel analysis.

🧹 Getting the Data in Shape

I loaded up Pandas, NumPy, Seaborn, and Matplotlib and pulled the dataset in:

import pandas as pd
import numpy as np
import seaborn as sns

nobel = pd.read_csv('datasets/nobel.csv')


From there, I cleaned up the date columns, fixed inconsistent country labels, and created new variables like whether a laureate was U.S.-born and their age at the time of receiving the award.

🔎 What I Found
1️⃣ Country Dominance Isn’t Static

In the early decades, Europe — especially the UK, Germany, and France — completely dominated.

But then things shifted.

2️⃣ The Rise of the United States

By tagging U.S.-born winners and plotting them by decade, the story became clear:

The U.S. starts pulling ahead in the 1930s and hasn’t looked back since.

This lines up with major scientific investment in the U.S. around that time, especially pre- and post-WWII.

3️⃣ Gender Imbalance Is… Severe

No surprises here, but seeing the numbers laid out decade by decade makes it even more striking.

For a long time, female laureates were extremely rare.

Things improve (slowly) in recent decades.

Peace and Literature show the most progress.

Physics and Economics? Still overwhelmingly male.

4️⃣ The First Woman: Marie Curie

It was nice to confirm that the very first female Nobel Prize winner was indeed Marie Curie in 1903 (Physics), and she later won another one in Chemistry.

She’s also one of the very few people ever to win twice.

5️⃣ Repeat Laureates Are Almost Mythical

Only a tiny group has won multiple Nobel Prizes, among them:

Marie Curie

John Bardeen

Linus Pauling

Frederick Sanger

The Red Cross & UNHCR

Most people never win one — winning two puts you in superhero territory.

6️⃣ Age Patterns Are Changing

By calculating age at the time of award, I noticed:

Early laureates were often in their early 50s.

Modern laureates are closer to their mid-60s.

Physics has the strongest trend toward older winners (maybe because cutting-edge breakthroughs take longer now?).

The Peace Prize is the opposite — it has gotten younger in recent years.

7️⃣ Youngest & Oldest

Youngest ever: Malala Yousafzai (17)

Oldest ever: Leonid Hurwicz (90)

The age spread is pretty wild.

📊 Bringing It to Life with Visuals

I plotted everything from U.S. dominance to gender proportions to age regressions across categories. Visuals made the century-long patterns much easier to spot and understand.

🔧 Tools I Used

Python for everything

Pandas for data wrangling

NumPy for numerical work

Seaborn + Matplotlib for charts

Nothing fancy — just the standard data analysis toolkit.

💡 What I Took Away

The global center of scientific and cultural influence really did shift to the U.S. in the 20th century.

Gender imbalance in Nobel Prizes is not only real — it’s massive.

Laureates are getting older, likely because modern research and discovery take longer.

Only a few people have achieved multiple Nobel wins, which shows how rare that kind of recognition is.

🚀 Want to Try It Yourself?
git clone https://github.com/devotuoma/A-Visual-History-of-Nobel-Price-Winners
pip install pandas numpy matplotlib seaborn


Open the notebook in Jupyter or VSCode and you’re good to go.
