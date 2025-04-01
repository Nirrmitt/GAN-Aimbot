VIDEO games attract millions of players, and the industry reports their revenue in billions of dollars. For instance, one of the biggest video game publishers, Activision Blizzard, reported more than 75 million players of their game Call of Duty: Modern Warfare (2019) and net revenue of over 3.7 billion US dollars in the first half of 2020. The gaming communities also contain e-sport tournaments with prize pools in millions, e.g. World Electronic Sports Games 2016 contained a prize pool of 1.5 million USD. With such popularity, cheating practices similar to doping in physical sports is commonplace in video games. For example, two public cheating communities have existed since 2000 and 2001, and have more than seven million members in total  and this is only a fraction of such communities. In these communities, users can share and develop different ways to cheat in multiplayer games. Although cheating is more difficult in in-person tournaments, cheating in online games is still prevalent. For example, UnknownCheats has 213 threads and more than a million views for the game Call of Duty: Modern Warfare (2019). The presence of cheaters degrades the user experience of other players, as playing with cheaters is not fun. Game developers are therefore encouraged to prevent such cheating. A common way to cheat in online games is by using tools and software (“hacks”) used by “hackers” , dating back to 1990 with the first forms of hacking with Game Genie . Hacking All authors are with School of Computing, University of Eastern Finland, Joensuu, Finland. V. Hautamäki is also with the Department of Electrical and Computer Engineering, National University of Singapore. E-mail: anssk@uef.fi, tkinnu@uef.fi, villeh@uef.fi is prohibited by game publishers, and they monitor players with anti-cheat software to detect hacking. A standard approach is to check running processes on the player’s computer for known cheating software—similar to how antivirus scanners look for specific strings of binary on a machine. The publisher can also analyse players’ behaviour and performance to detect suspicious activity, such as a sudden increase in a player’s performance. While hacks can be hidden from the former detection approach, the latter cannot be bypassed, as the system runs on game servers.
. Analysis of player behaviour is thus an attractive option for publishers. These data-based anti-cheats have also attracted the attention of the academic community, as well as from the game industry. Galli et al. (2011) developed hacks that provide additional information to the player and move the mouse in the game Unreal Tournament III. The authors then used machine learning to distinguish these hackers from legitimate players. Hashen et al. (2013)  extended this work by evaluating the accuracy of different classifiers versus different hacks. Yeung and Lui (2008) analysed players’ performance and then used Bayesian inference to analyse players’ accuracy and classify if a player was hacking.
All of these works have focused on detecting hackers with machine learning, but little attention had been given to cheating with machine learning. Yan and Randell have mentioned the use of machine learning for cheating, but only in the context of board games like Chess and Go and not in video games. Recent advances in machine learning allow one to generate photorealistic imagery , speech to attack voice biometric systems [10] or computer agents that mimic the demonstrators. Similar methods could be applied to video games to generate human-like gameplay. We define “human-like gameplay” as artificially generated gameplay that is indistinguishable from genuine human gameplay, either by other humans or by automated detection systems. If used for cheating, these methods threaten the integrity of multiplayer games, as the previously mentioned anti-cheat systems could not distinguish these cheaters.

 TABLES

Table 1Ethical Implications of GAN-Aimbots
Table 2 EVALUATION RESULTS OF DETECTING AIMBOTS.
Table 3. LIST OF COMMON ANTI-CHEAT SOFTWARE FOUND IN GAMES

1:-  Generative Adversarial Networks (GANs)


![Picture1](https://github.com/user-attachments/assets/413a6122-c360-45eb-a3a8-c4c0406040af)

Generative modeling is an unsupervised learning task in machine learning that involves automatically discovering and learning the regularities or patterns in input data in such a way that the model can be used to generate or output new examples that plausibly could have been drawn from the original dataset.

GANs are a clever way of training a generative model by framing the problem as a supervised learning problem with two sub-models: the generator model that we train to generate new examples, and the discriminator model that tries to classify examples as either real (from the domain) or fake (generated). The two models are trained together in a zero-sum game, adversarial, until the discriminator model is fooled about half the time, meaning the generator model is generating plausible examples.

GANs are an exciting and rapidly changing field, delivering on the promise of generative models in their ability to generate realistic examples across a range of problem domains, most notably in image-to-image translation tasks such as translating photos of summer to winter or day to night, and in generating photorealistic photos of objects, scenes, and people that even humans cannot tell are fake.

ViZDoom
We use Doom (1993) via ViZDoom library [32] as a game, as depicted in Figure1 . Doom is one of the first FPS games. While dated, Doom still includes core mechanics of FPS games, namely navigating the map to find enemies and killing them by aiming and firing weapons. We chose this game and library as ViZDoom allows granular control over game flow while remaining lightweight, which allows us to distribute the data collection programs to participants over the Internet. The human players play games of “deathmatch” on a single map, where players have to score the highest number of kills to win. Everyone plays against each other. A single human player plays with six computer-controlled players of varying strength; some exhibit higher-than-normal mobility and speed, making them difficult targets to hit. Players can find weapons stronger than the starting weapon (a pistol), but most weapons require multiple hits before they kill a target, highlighting the need for accurate aiming. So-called “instant-hit” weapons are of the most interest to our work—the projectiles of these weapons hit the target location immediately. These weapons reward the accurate aiming of the player and benefit the most from the use of aimbots.
![Picture2](https://github.com/user-attachments/assets/a90caf50-a813-4056-bb87-697449bfb130)

ViZDoom environment used for the experiments. The player can also aim vertically in this implementation of Doom. Red and green boxes represent field-of-views of the aimbots, red for strong and GAN-Aimbot and green for light aimbot. Aimbots activate automatically when a target (white boxes) is inside the field-of-view. The white, green and red boxes are not visible to the player. 



