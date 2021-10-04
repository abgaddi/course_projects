# Tableau Visualization

[Link to Dashboard](https://public.tableau.com/app/profile/gabrielle.gaddi/viz/BTSlyricsovertime/Dashboard1)

# Written Analysis

**BTS Lyrics Over Time**

BTS is a Grammy nominated Kpop group that has been active since 2013 and have gained popularity abroad in recent years.  What sets them apart from majority of groups is that their lyrics are about youth experiences such as the fear of not knowing what you want to do with your life, losing a close friend, and learning to love yourself.  As they have released around 150 songs within 15 albums, this analysis looks at if and how their lyrics have changed over the years.

The dataset used is from Kaggle[^1] and includes all of BTS’s released songs with the album title, release date, lyrics translated to English, and other relevant sections.  The lyrics were further cleaned in a jupyter notebook to exclude ‘skits’, where the group members are talking amongst themselves, and instrumental songs with no lyrics.  Duplicate songs that appear on multiple albums were also removed to avoid multiple counts of the same lyrics.  After preprocessing the data, the top 30 most common lyrics amongst all BTS songs were extracted using NLTK and the frequency distribution function.  Overall, the word ‘love’ occurred the most, followed by ‘know’ and ‘let’. These most common words were then counted each time it appeared in the lyrics of a song and grouped together by year.

In order to visualize and determine any changes, a Tableau dashboard was created including a word cloud and histogram for each year that shows the frequencies of the most common BTS lyrics.  Additionally, the song title and the first four lines of lyrics where the most common word appears is included in the word cloud.  The word ‘love’ appeared at its highest frequency of 197 instances in the year 2018 and its lowest in 2020.  Although, this is possibly due to the fact that there were less songs released in 2020 compared to 2018.  It was also found that the lyric ‘girl’ had its highest frequency in 2014, but afterwards decreased each year until it did not appear in the years 2018-2019 at all.

Looking closer at the context of these lyrics illustrates the significant shift of the group’s message.  In the earlier years, the lyric ‘love’ and ‘girl’ were used in young, school crush type songs:

> *“wanna be **love**d…” – I Like It, 2013*
>
> *“I’m so hungry for your **love**” – Boy In Luv, 2014*
>
> *“I think about you all night **girl**” – 24/7=Heaven, 2014*

In comparison to 2018, the highest occurrence of ‘love’, the context of the lyric was used in self-love/appreciation rather than towards another person:

> *“I’m the one I should **love**” – Epiphany, 2018*
>
> *“I’m learning how to **love** myself” – Answer: Love Myself, 2018*
> 
> *“because I came to have so many things that I **love**” – Anpanman, 2018*

The decline of the lyric ‘girl’ may be from increased awareness and consideration for the fan’s preferred pronouns and to address an increased range of fanbase.  Another interesting observation was the way the lyrics like ‘dream’ was used in their first year and most recent year.  In 2013, ‘dream’ alludes to ambition and is used with uncertainty, much like the anxiety adolescents face when having to choose a career path:

> *“hey, what’s your **dream**?” – No More Dream, 2013*
> 
>*“my **dream** is gone, no time to breath” – N.O., 2013*
>
>*“I know it’s an unreasonable dream, but it’s my **dream**” – If I Ruled the World, 2013*

In 2020, the lyric ‘dream’ is also used with uncertainty but used in a more literal, fantasy connotation.  The difference in these songs is that the fear is more about being awaken from a dream:

>*“am I still in a **dream**?” – We Are Bulletproof: The Eternal, 2020*
>
>*“was it a **dream**?” – Stay, 2020*

In conclusion, BTS’s lyrics have changed from when they first debuted to their most recent album release.  As the group has grown and aged together, the message of their songs and lyrics seems to  reflect their experiences and have also grown with them.  They continue to write about love and their fears. While in their younger school days, their lyrics were about having a trivial crush and worrying about the future.  As they’ve become adults, their lyrics express a mature love for themselves, but their worry has changed into the fear of waking up and losing all they have.

[^1]: https://www.kaggle.com/kailic/bts-lyrics



