# Real Nerdy Stats

This Python project scrapes Rotten Tomatoes to compile the "Tomatometer" scores of movies discussed by the podcast [Blank Check with Griffin and David](https://blankcheckpod.com). It requires the packages **pandas** and **BeautifulSoup**.

You will need to have the **blank_check_rt.ipynb** Jupyter notebook and the **blank_check_addl.ods** spreadsheet in the working folder. Running the notebook will create a file in that folder called **blank_check_rt.csv** with the compiled stats. (I've also uploaded these contents to [Google Sheets](https://docs.google.com/spreadsheets/d/1Y2KnLLl1tnineLOUMjU4lOK7PS76i6O35zkGX-aewfQ/edit?usp=sharing).)

**Blank Check** covers both directors (on its main feed), and franchises (on its [Patreon feed](https://www.patreon.com/blankcheck/posts)). This can lead to duplication. For instance, James Cameron's film **Aliens** has been covered both as part of a Cameron series, and as part of an **Alien** franchise series. For certain uses -- e.g., calculating the average Rotten Tomatoes score of directors and/or franchises -- this is the desired behavior. There are other situations where you may wish to drop the duplicates. 

The "subject" of the miniseries has been entered as the podcast classified it, regardless of whether it technically qualifies. For instance, Barbra Streisand is not the listed director of **A Star Is Born** (1976), but it's included as part of the Streisand mini-series because that's how the podcast treated it. Similarly, on the Patreon side, **The Love Guru** is grouped together with the Austin Powers franchise.

Please note that scraping by its nature is unreliable. Temporary access errors are common, and repeated scraping can result in IP bans or other loss of access to the Rotten Tomatoes site.

Smell ya later, fartheads!
