---
name: education-radar
description: Weekly Monday scan of global education news with analysis of the three most important items (in English)
---

You are producing the "Education Radar": a weekly briefing, written entirely in English, on global education news. Today is Monday; cover the previous 7 days.

STEP 1 - Gather. Use WebSearch (mode "standard"; send several searches in the same turn, and use "extended" only if results are thin) and WebFetch to collect education news from around the world published in the last 7 days. Cover these areas: K-12 and primary/secondary policy; higher education and research funding; edtech and AI in education (including regulation, new tools, cheating/assessment debates); teacher workforce (shortages, pay, strikes); curriculum and assessment reform; inclusion, wellbeing and safety; international rankings and reports (OECD, UNESCO, World Bank, PISA/TALIS). Cover multiple regions: Netherlands/Europe, UK, US, Asia-Pacific, Africa, Latin America, Middle East. Also check reliable sources such as Education Week, The Guardian Education, Times Higher Education, Inside Higher Ed, The 74, EdSurge, Chalkbeat, UNESCO, OECD, NOS Onderwijs, Trouw, VO-raad. Prefer primary or reputable sources and verify dates; discard anything older than ~10 days.

STEP 2 - Select. From everything found, build a short "Also on the radar" list of 8-12 items (one line each: headline, region, source link). Then choose the THREE most important items. Judge importance by: scale of impact (number of students/teachers/institutions affected), policy or structural significance, novelty, and relevance to digital learning / edtech / the Dutch and European context (the reader works at LessonUp, a lesson platform for teachers).

STEP 3 - Analyse. For each of the three items write an analysis of about 150-200 words with: What happened (facts only, with source link); Why it matters; Context/background; What to watch next (and, where relevant, implications for teachers and for edtech/lesson platforms). Be balanced, flag uncertainty, do not invent facts or quotes, and do not reproduce long passages from articles.

STEP 4 - Education tip. Write one "Education tip for the LessonUp team": a practical, evidence-informed teaching tip (80-120 words) that colleagues at LessonUp (educators, content makers, product people) can use or share with teachers. Tie it to this week's news where natural, otherwise to a well-supported teaching practice (e.g. retrieval practice, formative assessment, active learning, classroom engagement, using AI responsibly). Include a concrete example of how it could look in an interactive lesson, and cite a source if you rely on research. Do not invent studies.

STEP 5 - Output. Format as Markdown with: title "Education Radar - week <ISO week number>, <date>"; a 2-3 sentence "Week in one glance"; "Top 3" with the analyses; "Education tip for the LessonUp team"; "Also on the radar" list. Then publish it to the website:
1. Work in C:\Users\janws\Claude\onderwijsradar (a git repo; remote origin is github.com/gsleraar-hue/education-radar). Save the briefing as docs/reports/<YYYY>-W<WW>.md (ISO week; no other file names).
2. Edit docs/reports.json (a JSON array, newest first): insert {"file": "reports/<YYYY>-W<WW>.md", "week": "<YYYY>-W<WW>", "date": "<YYYY-MM-DD>"} at the top. If an entry for that week exists, replace it instead of duplicating.
3. Run: git add docs && git commit -m "Education Radar <YYYY>-W<WW>" and git push. Commit only files under docs/. If the push fails, say so in the final message and do not retry destructively (no force-push).
Finally print the full briefing as your final message, followed by one line stating whether the site was updated (https://gsleraar-hue.github.io/education-radar/).
