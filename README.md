# genshin-wish-sim
a Genshin wish simulator that uses the in-game odds to generate accurate pulls and give an insight about the odds of the results
# This is a project which discusses and further analyzes the Gacha System and its probabilities.
# Since every Gacha Game differs in many ways, whether it's the rarity of items or their drop rates, 
# it makes sense to focus on the Gacha System of a singular game rather than generalizing the topic.
# For this project, we will be using the rarities and probabilities of the game "Genshin Impact".

# in the Genshin Impact Gacha System, the base probability to get a 5* Character lies at 0.6%, or 6 in 1000.
# additionally, the hard pity lies at 90, meaning if you reach the 90th pull, you will get a 5* with a 100% chance.

# following only those probabilities, our chances would look like this:
# Figure 1) shows the per-pull probability, speak: the individual probability at each pull x
# for example: 35: the chance to get a 5* at the 35th pull is 0.6%.
# it shows that starting at 1 and throughout 89, our chances lie at 0.6 %, and at 90, it increases to 100%.
# Figure 2) shows the cumulative probability, speak: the probability to get a 5* character up until that point.
# for example: 35: the chance to get a 5* character within 35 pulls is ~ 19%.
# it shows that if we count it together, we have a ~ 41 % chance to get our 5* character before reaching the 90th pull.

# however, if we compare the probabilities of Figure 1) and 2) with real player data (see Figure 5)), we can easily see that 
# most players get their 5* character close to the 77th pull, and an incredibly small number of players even reach the 90th pull
# (0.0003 %, which would be 3 players out of 100000 !)
# but why?

# this is because the Genshin Impact Gacha System has something called "soft pity".
# soft pity is a territory, specifically in the range of the 74th and 90th pull, where the probability of getting a 5* character 
# increases by the same amount with every pull.
# if our base probability is 0.6% and we know that the soft pity starts at 74 and has to reach 100% by the 90th pull,
# the only amount that makes sense is 6%.
# this means that when a player reaches the 74th pull, their chance for a 5* is increased by 6%, so 74th pull = 6.6%
# so if every next pull gains the same amount of chance, we would have the 75th pull with 12.6%, the 76th with 18.6% and so on.
# if every pull has an increased chance of 6%, we reach 96.6% at 89, and the first time we reach ~100% is at the 90th pull.
# (Full list at: https://ibb.co/QDcc5NJ)

# so if we consider soft pity, our per-pull probability looks like Figure 3) and our cummulative probability like Figure 4),
# which looks a lot more like our actual player data!
