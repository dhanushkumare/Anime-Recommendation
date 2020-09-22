# Anime-Recommendation
A Recommendation system specifically for anime nerds. 


[Dataset downloaded from Kaggle](https://www.kaggle.com/CooperUnion/anime-recommendations-database)

## Problem Statement:
>I'm in need of some anime series recommendations that are under 100 episodes. I'm fairly new to anime so I don't know the exact genre/type I'm looking for, although I have >enjoyed all that i have watched so far.
>Things Ive enjoyed about the ones I have seen and are particularly looking for are:
>- Good plot lines and twists (e.g Death note, Steins Gate)
>- Male protagonists that are strong overpowered but aren't entirely full of themselves (e.g Kirito from Sword Art Online, Rin from Ao no Exorcst, Roy Mustang from >FMA:Brotherhood)
>- Reasonably modern animation art
>- Fantasy, Supernatural, Action, Adventure
>Things I'm not really interested in unless highly recommended to watch:
>- Sports themed
>- High school as main theme
>- Vampires
>- Too much like real life
>- Too much mecha (Enjoyed Code Geass)
>- Too much ecchi (Enjoyed Elfin Lied)
>Suggestions much appreciated :)

This is an example of one of the comments posted by the user on myanimelist.net. Why do people rely on others to choose their movies/shows? They assume that there might be a group of people who might have similar interests to them and they can suggest some shows the user may like. Instead of posting comments like these everytime and waiting for someones response seems like a tedious task. If we can find the similarities based on the users behavioural pattern and recommend shows based on the users interest the user may like our product and they might suggest to their friends/families. So from a pure business perspective we need to retain the existing customers and add customers to our product to increase our revenue.

## Solution to the users comment on a high level

>- Need anime series under 100 episodes
>- Likes Death Note and Steins Gate
>- Likes genre Fantasy, Supernatural, Action, Adventure

Death note has 37 episodes and Steins Gate has 25 episodes in total. This implicitly says that the user likes animes which are short in number. We will have a feature based on the number of episodes the anime has. Both falls under thriller genre. So we can recommend shows which are under 50 episodes and falls under a thriller genre. The user also likes action, adventure, fantasy and supernatural genres. So we can recommend anime which falls under this genre and they have less than 50 episodes.
This is an example of *Content Based filtering*. These features are explicitly based on the users preference.

What if we find an user m who likes anime such as  `Steins Gate` , `Death Note` , `Another` and likes genre such as thriller , action and horror ? We can recommend all the shows which are liked by user m to our user because they have similar show and genre preference. This is an example of *Collobrative filtering*. These features are based on other users preference.

## Objective
The main objective of this project is to recommend similar anime to the end users by using techniques like Collobrative filtering. Since we dont have that much of an information about the user or anime ,solving this problem using Content Based filtering is a little bit difficult.
