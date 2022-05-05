---
layout: descrip
title: Similar Singer
description:
img: /assets/img/simsing.jpg
importance: 1
category:
---

# Similar Singer

Product Manager & Backend / February 2021 to May 2021

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="center" src="{{ '/assets/img/simsing2.jpg' | relative_url }}" alt="" title="similar singer"/>
    </div>
</div>
<div class="caption">
    Similar Singer
</div>

[Similar Singer](https://similarsinger-final.herokuapp.com/) is a musical artist recommendation engine that allows users to get new artist and song recommendations based on their current musical preferences. As a final project for CS 4300: Language and Information, it served as the culminating experience of months of work within a remote team.

I was the PM and backend developer on the project and helped lead a group of 5 from ideation to launch in 3 months.

---

**Overview**

**Problem**

We wanted to create a useful recommendation system that could be a tool in the everyday lives of people.

After speaking with friends, family, and others, we identified possible improvements to how music is currently recommended. Mainly done through screaming platforms, services like Spotify’s Related Artists and Apple Music’s recommendations give suggestions for popular artists based on their shared listeners and genre, but do not take other user preferences into account.

How might we…
1. Create a platform that is personalized and gives the users recommendations that are more tailored to their tastes?
2. Allow users to specify the type of songs they want?
3. Give users the option to sample these songs and immediately access new music?

**Team**

We were a small team of 5:
- Me, PM & Data Back-End
- Celine: Front-End
- Alyssa: Web & Data Back-End
- Mahak: Front-End
- Jasper: Web Back-End

**Timeline**

We started brainstorming in mid-March and launched the final version of [Similar Singer](https://similarsinger-final.herokuapp.com/) mid-May.

**Outcome**

Features:

- User can input multiple liked and disliked artists
- User can give a description of the type of music/artist they want to see with a linguistic descriptor
- Analysis of lyric and genre similarity to find best match for user
- Similarity score of results to user’s preferences
- Information about recommended artists
- Genres
- Ranked similarities to user’s preferences
- Spotify submodule of top songs and followings
- Pitchfork album reviews and ratings

**Product**

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="center" src="{{ '/assets/img/image1.jpg' | relative_url }}" alt="" title="image1"/>
    </div>
</div>
<div class="caption">
    Final Results
</div>

**Co-building with users**

We made numerous prototypes and tested them with users to get their feedback.

Key takeaways:

- Our initial instinct was to utilize just cosine similarity and natural language processing, but those did not impact the results as much as we thought.
- The Heroku platform was finicky at times, and getting + maintaining data from Spotify and Pitchfork was trickier than expected.
- We initially had lyric similarity and genre similarity weighted equally, but after speaking with potential users, they wanted genre to be weighed heavier.
- Users like the ability to have suggested artists and play songs right away.

**Challenges**

The biggest challenge came from working in multiple different time zones and making sure that we kept making progress. To consistently meet and align goals and responsibilities, we had weekly meetings and milestone submissions. I directed the group and organized the direction of these sessions, working to resolve issues methodically. I also acted to prioritize key product features and capabilities, thinking about the user first.

Technical Updates:
- When a user is interested in music without lyrics, we need to prioritize the genre of their liked artist
- Social Component: users want to see artists that other similar users also listen to, so we realized we needed to incorporate shared followers
- Utilizing machine learning with an LDA model with a tokenized, lemmatized corpus of around 1,200 Pitchfork albums: topic modeling with a much larger corpus from both Amazon and Pitchfork resulted in non-English language reviews
- Dynamic: using the rocchio update algorithm, we combined the liked and disliked artists from the user to vectorize their preferences

**Launch**

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="center" src="{{ '/assets/img/milestone1.jpg' | relative_url }}" alt="" title="milestone1"/>
    </div>
</div>
<div class="caption">
    First Demo
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="center" src="{{ '/assets/img/milestone2.jpg' | relative_url }}" alt="" title="milestone2"/>
    </div>
</div>
<div class="caption">
    Second Demo
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="center" src="{{ '/assets/img/finalmilestone1.jpg' | relative_url }}" alt="" title="final1"/>
    </div>
</div>
<div class="caption">
    Final Results with Songs
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="center" src="{{ '/assets/img/finalmilestone2.jpg' | relative_url }}" alt="" title="final2"/>
    </div>
</div>
<div class="caption">
    Final Product
</div>

Links:

[First Demo](https://similarsinger.herokuapp.com/ )

[Second Demo](https://similarsinger-prototype2.herokuapp.com/ )

[Final Product](https://similarsinger-final.herokuapp.com/ )


**Impact**

Our final product culminated in a user experience that many wanted to recommend to their friends and family. The integration of Spotify and Pitchfork made it easy for users to find songs and albums immediately. Users updated their playlists and libraries immediately.

**Learnings**

- Teamwork: Team members all need to work together and communicate roles. You have to be there to help ensure that your members feel supported and able to express their ideas.
- Problem Solving: From the moment we started the project, every part involved some sort of adaptation and adjustment to road blocks. Taking these strides in place and learning how to fix issues without changing the original goal meant using analytical skills and flexibility.
- Technical: The overall scope of the project involved many moving parts and concepts, including machine learning, natural language processing, data science, and web development. If there was something we did not understand, we did not hesitate to ask each other or do research.
- Communication: Platforms like Zoom and Slack made it a lot easier to meet with group members, but group meetings were key to our success. I outlined agendas and came in with how we needed to adapt to user needs. When we left these meetings, we had clear goals and how to shift.
- Presentation: Users like a clean, usable product. We created a design that looked aesthetically pleasing but also conveyed a lot of information without being overwhelming. I learned that having an intuitive product is key to success.
