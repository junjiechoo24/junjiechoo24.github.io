---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
classes: wide
---

<hr>

# Journal App: N=1 Research to investigate correlations between Journaling and Psychological Well Being over time

<a href="[View Live Application](https://6885ec796d69eab0ccece44d--glowing-dolphin-ed108f.netlify.app/)" target="_blank" rel="noopener noreferrer"></a>

Feel free to test it out with these credentials:

Email: testuser@gmail.com
<br>
Password: journalapptest

<img width="1547" height="1112" alt="image" src="https://github.com/user-attachments/assets/c9af412b-047a-4a45-8546-7969eec9dac9" />

This is a full-stack web application I designed to track my personal psychological well-being scores and how it correlates with journaling, it is essentially a mixed-methods N=1 study. It combines qualitative journal reflection entries with quantitative, validated psychological scales, e.g: Flourishing Scale (Diener et al., 2010) to track and analyse the drivers of personal well-being.

## Core Features & Methodology

### 1. Journal
A daily journaling prompt with four open-ended questions designed to foster self-reflection and narrative coherence.
*   *Something that happened*
*   *Something you did well*
*   *What did not go well*
*   *The bigger picture*

![Screenshot of the Journaling Page](https://github.com/user-attachments/assets/1786dac8-87af-4eac-b795-b817e08a80cf)

### 2. The Daily Flourishing Scale
A daily, 5-item questionnaire answered every evening. The items are adapted from the comprehensive Harvard Flourishing Measure to provide a sensitive, day-to-day "pulse" of well-being across five key domains.

![Screenshot of the Daily Flourishing Scale Page](https://github.com/user-attachments/assets/b6cc2690-34b1-40f6-9648-acd3340db111)

### 3. The Weekly Flourishing Scale
The full, 8-item Flourishing Scale (Diener et al., 2010) is administered once per week to track stable, long-term changes in overall psychological well-being.

![Screenshot of the Weekly Flourishing Scale Page](https://github.com/user-attachments/assets/b0fe63c3-30cf-4b72-9c57-3e84c1b1085e)
---

## Technical Architecture

This project is built with a modern, secure, and scalable full-stack architecture.

### Front-End
*   **Framework:** **React** (built with Vite)
*   **Routing:** **React Router** for multi-page navigation.
*   **Styling:** Custom CSS for a clean, minimal, and responsive UI.
*   **Deployment:** Hosted on **Netlify** with continuous deployment via GitHub.

### Back-End
*   **Database:** **Supabase** (PostgreSQL)
*   **Authentication:** **Supabase Auth** for secure user login.
*   **Security:** **Row Level Security (RLS)** is enabled on all tables, with policies that ensure users can only ever access their own data.

### Future Improvements
*   To include data visualisation of well-being scores
*   To include data insights of journal entries and well-being scores

<a href="https://github.com/junjiechoo24/journal-app" class="btn" target="_blank" rel="noopener noreferrer">View Code on GitHub</a>
