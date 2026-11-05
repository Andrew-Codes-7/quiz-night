# Quiz Night

A free trivia game for 1 to 4 players: set up players, pick a category, and race the clock. Part of [Emerald City Apps](https://emeraldcityapps.com).

**Play it:** [quiz.emeraldcityapps.com](https://quiz.emeraldcityapps.com)

## Features

- 1 to 4 players taking turns, with rounds and a countdown timer
- Categories including Flags, Country Shapes, Capitals, World History, Stadiums, City Skylines, Cities from Space, Music, Spanish and General Knowledge
- A Kids Zone with longer timers and a hint on every question
- Best scores remembered between games, and a "Share my score" button

The logo-based quizzes (Team Logos, Company Logos and Pixelated Logos) are switched off for the public version, and Career Paths shows team names and years instead of logos. Set `SHOW_LOGO_QUIZZES` to `true` in `index.html` to bring the logos back.

Pictures live in `images/`. Most are free photos from Wikimedia Commons, credited in the game after each answer. `images/disney` and `images/movies` are drop-in folders: save a picture there using a file name from that folder's `LIST.txt` and it joins the Pixelated rounds.

## Tech

A single HTML file with vanilla JavaScript and CSS. No build step and no account; scores are saved in the browser with `localStorage`. `_headers` sets the security headers on Netlify.

## Running it

Open `index.html` in a browser. Deploys to Netlify automatically on every push to `main`.
