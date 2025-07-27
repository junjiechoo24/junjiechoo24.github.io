---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
classes: wide
---

<hr>

## Journal App: A Mixed-Methods Tool for N=1 Research

<a href="[View Live Application](https://6885ec796d69eab0ccece44d--glowing-dolphin-ed108f.netlify.app/)" target="_blank" rel="noopener noreferrer"></a>

Feel free to test it out with these credentials:

Email: testuser@gmail.com
Password: journalapptest

<img width="1547" height="1112" alt="image" src="https://github.com/user-attachments/assets/c9af412b-047a-4a45-8546-7969eec9dac9" />

This is a full-stack web application I designed to track my psychological well-being scores and how it correlates with journaling, it is essentially a mixed-methods N=1 study. It combines qualitative journal reflection entries with quantitative, validated psychological scales, e.g: Flourishing Scale (Diener et al., 2010) to track and analyse the drivers of personal well-being.


#### Key Features & Methodology
*   **Secure User Authentication:** Full login/logout functionality built with Supabase Auth.
*   **Role-Based Security:** Row Level Security (RLS) is enabled on all tables, with policies ensuring users can only ever access their own private data.
*   **Qualitative Data Collection:** A multi-prompt journaling form for narrative entries.
*   **Quantitative Data Collection:** Custom, interactive forms for validated scales, including a daily "Flourishing Index" adapted from a flourishing scale from Harvard and the weekly Flourishing Scale (Diener et al., 2010).

#### Tech Stack
*   **Front-End:** **React** (built with Vite)
*   **Routing:** **React Router**
*   **Back-End & Database:** **Supabase** (PostgreSQL)
*   **Deployment:** **Netlify** (with Continuous Deployment from GitHub)

<a href="https://github.com/junjiechoo24/journal-app" class="btn" target="_blank" rel="noopener noreferrer">View Code on GitHub</a>
