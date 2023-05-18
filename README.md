# # Modified Chicken Game under a Spy Operation Scenario
## Project information
- **Author**: Yuchen Song, Computation and Design with tracks in Computer Science, 2025, Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: Submissions to the Final Project for [COMPSCI/ECON 206 Computational Microeconomics, 2023 Spring (Seven Week - Second)](https://ce.pubpub.org/) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Project Summary**: 
  - Summarize the Background/Motivation: Nash equilibrium is based on the assumption that players are rational, but in reality, players are sometimes willing to take risks to maximize profit. For example, in Chicken Game, the solution obtained by using Nash equilibrium is that both sides choose chicken, but one side may bet that the opposite side is rational and will choose chicken. Based on this risky assumption, he will choose Dave to maximize his own payoff. Therefore, based on the discussion of spy in the Art of War, this paper proposes a solution concept to avoid irrational self-interest maximization and increase the probability to choose a Nash equilibrium strategy.
  - Research Questions: 1. Are there some ways to force both players to be perfectly rational in the game, ultimately increasing the probability that the players will choose the Nash equilibrium? 2. How will people act in the modified Chicken Game? What are their rationales? 3. Can the additional rules in the game influence people’s decision-making and force them to avoid risk-taking choices and choose the Nash equilibrium?
  - Application Scenario: The modified Chicken Game can be applied to situations involving conflicts or interactions between two sides where risk-taking and risk-avoidance are key elements. Examples includes business negotiations, military deterrence and political game. 
  - Methodology:The game is based on a classical game in game theory literature, Chicken Game, which is a model of conflict between risk-taking and risk-avoidance of two players. In the modified version, one additional rule is that both players can choose whether to spy at the beginning of the game, if so, he will pay 1 payoff at last. The game has two rounds, and the total payoff is the sum of the payoff in two rounds.
  - Results: Based on the modified game and the analysis of all strategies, the optimal strategy is not the one suggested by Nash Equilibrium.
  - Intellectual Merits and Practical impacts: Experiment verifications, a more complex game environment containing spy actions, extension to other strategic form games, and psychological and behavioral studies are future research directions based on this research
  
   
Note: please insert the screenshot of the answers to your research question by ChatGPT. The methodology that you use to address the research questions must be more innovative than both the current literature and ChatGPT. 

## Table of Contents

- polished problem set 1 and problem set 2
- model
- code
- spotlight
- more about the author
- references

### Polished PS1 and PS2

- Polished Problem Set 1: [CS206-ECON206-Yuchen-Song-PS1](https://github.com/Rising-Stars-by-Sunshine/CS206-ECON206-Yuchen-Song-PS1)
- Polished Problem Set 2: [csecon206-Yuchen-PS2](https://github.com/Rising-Stars-by-Sunshine/csecon206-Yuchen-PS2)

### Model
- Game Environment: 
  
  The game is based on a classical game in game theory literature, Chicken Game, which is a model of conflict between risk-taking and risk-avoidance of two players. One of the classical game scenarios is when two drivers drive toward each other, each can choose to swerve or straight. If one of them chooses to swerve and the other chooses to straight, the former one will be seen as chickening out and will receive a lower payoff (2), while the latter one will receive a higher payoff (7) since he’s braver. If both choose to swerve, it will be a tie, and both receive a moderate payoff (6,6). While, if both players choose to straight, they will crash into each other, and receives a zero payoff, since they fail to avoid the risk. In the modified version, one additional rule is that both players can choose whether to spy at the beginning of the game, if so, he will pay 1 payoff at last. The game has two rounds, and the total payoff is the sum of the payoff in two rounds.
- Solution Concept: 
  
  In the first case, neither side uses spies, and in the last case, there are two possible scenarios. One, both are rational, and the payoff is (12,12). Second, when one hopes to maximize the payoff in one or two rounds, the payoff is (13,8) or (14,4). Three: Both people are hoping to maximize the payoff in one or two rounds, the payoff being (9,9) or (0,0) or (7,2), or (2,7). It is worth mentioning that in the third scenario, it is possible for one party to retaliate against the other party in the second round due to the other party's selfish choice in the first round. Both (7,2) and (9,9) could be the payoff of this scenario. 
  
  In every other case, at least one party used a spy in at least one round. Note that if spies are used, players will let each other know about the spy operation, because if not telling their opponent, the payoff of 1 won't affect their strategy except to know the other's choice ahead of time.  
  
  The second scenario is that one party (let's say player A) used A spy in the first round, then based on the above analysis, Player A will inform Player B, and Player B may choose to retaliate against Player A's spy because using a spy is a sign of distrust, so the result of this round is (-1, 0) or (1,7). In this case, the payoff will be less than 21, regardless of whether the two parties use spies in Round 2. 
  
  The third scenario is that both parties used spies in the first round, so they both know the other used spies. In these situations, where each partner's choices are being monitored by the other, and each knows that the other doesn't trust them, the chances that one of them will take a risk are greatly reduced. Because he knows that his behavior is being monitored, he knows that if he chooses to maximize his own interests, the other party will be more likely to retaliate against his irrational choice based on distrust. In this case, both parties are more likely to choose to swerve when they are subject to such constraints, and the yield of this round is (5,5). In Round 2, if both sides choose to use spies, it is likely that (10,10) total payoff will be reached based on the previous analysis. 
  
  In all three cases, we found that spying may be seen as a sign of distrust, increasing the likelihood of retaliation, but when both parties spy and their actions are monitored, players are less willing to take risks and retaliate accordingly. So, both sides should choose to use spies to get a (10,10) payoff with a high probability, even if a payoff of 4 is consumed. If both do not use spies the total return is likely to be lower than 22, with the risk of having a very low, and unfair payoff. So, in general, we've had a smaller payoff for a more stable and equitable payoff.

- Evaluations: 
  
  If we analyze this modified game by Nash Equilibrium, it will suggest both players not use spies and be rational to choose swerve, which results in a (6,6) payoff. However, according to the analysis above, it is difficult for players to be perfectly rational, especially under the additional rules. Therefore, using spies for both players to raise the probability of achieving a fair and more stable equilibrium with little cost is a preferable solution to what Nash equilibrium suggests.

### Code
- [Overleaf Project](https://github.com/Rising-Stars-by-Sunshine/CS-ECON206_Yuchen_Song_Final_Project/blob/main/code/CSECON206_Final_Project_Spring2023_Yuchen.pdf)
- [Colab Project]()

### Spotlight
- Posters

![image](https://github.com/Rising-Stars-by-Sunshine/CS-ECON206_Yuchen_Song_Final_Project/blob/main/spotlight/Attack%20%26%20Defense%20Game%20A%20Simulation%20and%20Modeling%20of%20Two-side%20Confrontation%20Scenarios.png)
- Slides

[Econ206 Final Project.pptx](https://github.com/Rising-Stars-by-Sunshine/CS-ECON206_Yuchen_Song_Final_Project/blob/main/spotlight/Econ206%20Final%20Project.pptx)


### More about the Author
- headshot

![image](https://github.com/Rising-Stars-by-Sunshine/CS-ECON206_Yuchen_Song_Final_Project/blob/main/spotlight/headshot%20(1).jpg)
- self-introduction
  
  Yuchen Song is a sophomore student majored in Computation and Design with tracks in Computer Science at DKU, who is intereted in the intersection between Computer Science and other subjects.
- Final reflections 
  - intellectual growth

    Through this project, I found that interdisciplinary research could enable me to analyze the concepts of game theory from different perspectives. For example, from the point of view of psychology and behavioral science, the Nash equilibrium's assumption that players are absolutely rational is not true. From a computer science perspective, there are many programming techniques we can use to simplify Nash Equilibrium calculations and simulate game environments. At the same time, based on the interdisciplinary research of game theory and other disciplines and the improvement of existing theories, it is applied to different disciplines and brings inspiration to the research of other disciplines.
  
  - professional growth

    In this course and research, I have understood and learned the software related to game theory, such as SPNE and Otree. At the same time, I have learned relevant programming knowledge, such as Nashpy and Latex. I have also learned the basic process of editing and writing academic papers. These knowledge will be of great help to my future research and study.
    
  - living a purposeful life

### References

- Literature References in [Chicago Author-Date](https://www.chicagomanualofstyle.org/tools_citationguide/citation-guide-2.html) Style and [BibTex](https://scholar.google.com/) 

Levin, Dan, and Luyao Zhang. 2020. “Bridging Level-K to Nash Equilibrium.” *The Review of Economics and Statistics* 104 (6): 1329–40. https://doi.org/10.1162/rest_a_00990.

```
@book{tzu2012sun,
  title={Sun Tzu's The Art of War: Bilingual Edition Complete Chinese and English Text},
  author={Tzu, Sun},
  year={2012},
  publisher={Tuttle Publishing}
}
@article{niou1994game,
  title={A Game-Theoretic Interpretation of Sun Tzu's: The Art of War},
  author={Niou, Emerson MS and Ordeshook, Peter C},
  journal={Journal of Peace Research},
  volume={31},
  number={2},
  pages={161--174},
  year={1994},
  publisher={Sage Publications 6 Bonhill Street, London EC2A 4PU, UK}
}
@article{rapoport1966game,
  title={The game of chicken},
  author={Rapoport, Anatol and Chammah, Albert M},
  journal={American Behavioral Scientist},
  volume={10},
  number={3},
  pages={10--28},
  year={1966},
  publisher={Sage Publications Sage CA: Thousand Oaks, CA}
}
@article{nash1950equilibrium,
  title={Equilibrium points in n-person games},
  author={Nash Jr, John F},
  journal={Proceedings of the national academy of sciences},
  volume={36},
  number={1},
  pages={48--49},
  year={1950},
  publisher={National Acad Sciences}
}
@article{asch1956studies,
  title={Studies of independence and conformity: I. A minority of one against a unanimous majority.},
  author={Asch, Solomon E},
  journal={Psychological monographs: General and applied},
  volume={70},
  number={9},
  pages={1},
  year={1956},
  publisher={American Psychological Association}
}
```

