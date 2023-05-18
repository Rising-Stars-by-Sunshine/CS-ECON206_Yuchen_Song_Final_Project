# # Modified Chicken Game under a Spy Operation Scenario
## Project information
- **Author**: Yuchen Song, Computation and Design with tracks in Computer Science, 2025, Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: Submissions to the Problem Set No. or Final Project for [COMPSCI/ECON 206 Computational Microeconomics, 2023 Spring (Seven Week - Second)](https://ce.pubpub.org/) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Project Summary**: 
  - Summarize the Background/Motivation: Nash equilibrium is based on the assumption that players are rational, but in reality, players are sometimes willing to take risks to maximize profit. For example, in Chicken Game, the solution obtained by using Nash equilibrium is that both sides choose chicken, but one side may bet that the opposite side is rational and will choose chicken. Based on this risky assumption, he will choose Dave to maximize his own payoff. Therefore, based on the discussion of spy in the Art of War, this paper proposes a solution concept to avoid irrational self-interest maximization and increase the probability to choose a Nash equilibrium strategy.
  - Research Questions: 1. Are there some ways to force both players to be perfectly rational in the game, ultimately increasing the probability that the players will choose the Nash equilibrium? 2. How will people act in the modified Chicken Game? What are their rationales? 3. Can the additional rules in the game influence people’s decision-making and force them to avoid risk-taking choices and choose the Nash equilibrium?

  - Application Scenario: The modified Chicken Game can be applied to situations involving conflicts or interactions between two sides where risk-taking and risk-avoidance are key elements. Here are some examples. In business negotiations, the game can be used to simulate conflicts during a two-sided business negotiation. For each side, they should decide whether to take a risk-taking strategy or a risk-averse strategy. The decision of spying can be seen as gathering information from an insider during the negotiations. Another application scenario is military deterrence. If one side chooses to take risks, he will choose to threaten the other side, but there is a risk that the other side will start a war with him. If one party chooses to avoid risks, he may be threatened by the other party and get a lower payoff in the negotiation. The spy option is the spy in the real situation, he can help his side to know the other side's actions and choice tendencies.
  - Methodology:The game is based on a classical game in game theory literature, Chicken Game, which is a model of conflict between risk-taking and risk-avoidance of two players. One of the classical game scenarios is when two drivers drive toward each other, each can choose to swerve or straight. If one of them chooses to swerve and the other chooses to straight, the former one will be seen as chickening out and will receive a lower payoff (2), while the latter one will receive a higher payoff (7) since he’s braver. If both choose to swerve, it will be a tie, and both receive a moderate payoff (6,6). While, if both players choose to straight, they will crash into each other, and receives a zero payoff, since they fail to avoid the risk. In the modified version, one additional rule is that both players can choose whether to spy at the beginning of the game, if so, he will pay 1 payoff at last. The game has two rounds, and the total payoff is the sum of the payoff in two rounds.
  - Results: If we analyze this modified game by Nash Equilibrium, it will suggest both players not use spies and be rational to choose swerve, which results in a (6,6) payoff. However, according to the analysis above, it is difficult for players to be perfectly rational, especially under the additional rules. Therefore, using spies for both players to raise the probability of achieving a fair and more stable equilibrium with little cost is a preferable solution to what Nash equilibrium suggests.
  - Intellectual Merits and Practical impacts: This study has limitations in the following aspects. First, the game only discusses the situation in that both sides can choose to use or not use a spy, but in reality, there are double-sided or multi-sided spies, more than one spy, their own spy betrays, and other complex situations. Discussing these situations can be very complicated because they cause an imperfect information game to become an incomplete information game. In this type of game, players worry about how much and how accurately others are getting information about them. As a result, not only will players choose according to the payoff, but there will be issues of manipulating information. Second, the study assumes that player strategy choices are based on knowledge of behavior and game theory, but no experiments have been conducted, so we cannot test the theory. During the experiment, data may appear that is different from the theory, or factors may arise that affect the player in ways that are not anticipated.
  
   
Note: please insert the screenshot of the answers to your research question by ChatGPT. The methodology that you use to address the research questions must be more innovative than both the current literature and ChatGPT. 

## Table of Contents

- polished problem set 1 and problem set 2
- model
- code
- spotlight
- more about the author
- references

### Model
- Game Environment
- Solution Concept
- Evaluations: e.g. efficiency and fairness

### Code
- Game Environment
- Strategic plays
- Equilibruim Evaluations: e.g. belief, strategy, and payoffs
- oTree Experimental Code 


### Spotlight
- Posters
- Figures
- Slides
- Presentations
- Review articles
- Media appearance

### More about the Author
- headshot
- self-introduction
- Final reflections 
  - intellectual growth
  - professional growth
  - living a purposeful life

### References

- Literature References in [Chicago Author-Date](https://www.chicagomanualofstyle.org/tools_citationguide/citation-guide-2.html) Style and [BibTex](https://scholar.google.com/) 

Levin, Dan, and Luyao Zhang. 2020. “Bridging Level-K to Nash Equilibrium.” *The Review of Economics and Statistics* 104 (6): 1329–40. https://doi.org/10.1162/rest_a_00990.

```
@article{levin2022bridging,
  title={Bridging level-k to nash equilibrium},
  author={Levin, Dan and Zhang, Luyao},
  journal={Review of Economics and Statistics},
  volume={104},
  number={6},
  pages={1329--1340},
  year={2022},
  publisher={MIT Press One Rogers Street, Cambridge, MA 02142-1209, USA journals-info~…}
}
```

