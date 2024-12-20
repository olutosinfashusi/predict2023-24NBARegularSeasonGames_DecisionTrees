# PREDICT RESULTS OF 2023-24 NBA REGULAR SEASON GAMES WITH DECISION TREES
## BY OLUTOSIN FASHUSI
<b><i> EXCERPT FROM NBA GAMES PLAYED ON 2024-02-22: </b></i>
<br><br>
![matchResults](https://github.com/user-attachments/assets/3f5fb5a9-f76c-493d-a1ad-0ae9d00fb74a)
• DATE: Date game played (Predictions start on games played post the 2024 All Star Game which was played on 2024-02-18) <br>
• MATCH: Team abbreviation of away team @ team abbreviation of home team <br>
• GAMEID: Every NBA game has a unique GAMEID <br>
• MODEL PREDICTS: Team abbreviation that model predicts to win <br>
• ACTUAL WINNER: (Team abbreviation that actually won the game, ✅ if model vs actual winner model prediction correct ❌ if incorrect) <br>
• BETTING FAVORITE: (Team abbreviation of betting favorite, match spread, ✅ if model vs betting favorite model prediction correct ❌ if incorrect)
# MATCH TRAIN & TEST DETAILS AND DECISION TREE PLOTS
## MATCH ORL @ CLE, GAMEID: 22300792 TRAIN & TEST DETAILS 
![ORL@CLEMATCHRESULTS](https://github.com/user-attachments/assets/2fec338a-4670-4e74-b5ab-29a50ed1a041)
![ORL@CLE_TESTDETAILS](https://github.com/user-attachments/assets/8cf433f3-4ffe-405c-993a-39ca1ef52a8f)
• TRAIN SIZE: Number of applicable previous games used to train model  <br>
• SPLIT DETAILS: {Tree Depth: ('Feature', Threshold value)} <br>
• X_test: [(Feature Name, Feature Value, Tree Decision)]<br>
&nbsp;&nbsp;&nbsp; F indicates less than or equal to feature value (<=) is false so final node is left side <br>
&nbsp;&nbsp;&nbsp; T indicates less than or equal to feature value (<=) is true so final node is right side <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH ORL @ CLE, GAMEID: 22300792 DECISION TREE PLOTS
![ORL@CLE_TREE](https://github.com/user-attachments/assets/75d39d04-6199-436d-ace1-3db7f6dcd06b)
<br>
• Model identifies Field Goals Made (Unassisted) in last 3 games played (FGM %UASTL3MA) has lowest weighted Gini Impurity & best split for team, ORL (Orlando Magic) <br>
• Model identifies Percent of Points (Off Turnovers) in last 5 games played (%PTS OFF TOL5MA) has lowest weighted Gini Impurity & best split for team, CLE (Cleveland Cavaliers)
## MATCH ORL @ CLE, GAMEID: 22300792 WEIGHTED GINI IMPUTITIES
![ORLWGIs](https://github.com/user-attachments/assets/68e091e0-3ee3-4fb8-aee0-e8746b4acd03)
![CLEWGIs](https://github.com/user-attachments/assets/4689002c-3b64-454b-9fee-c001c00a3d6f)
<br><br>
## MATCH DET @ IND, GAMEID: 22300793 TRAIN & TEST DETAILS
![DET@IND_MATCHRESULTS](https://github.com/user-attachments/assets/1b7ab63c-f60b-4f8b-acbd-553356b7f5ee)
![DET@IND_TESTDETAILS](https://github.com/user-attachments/assets/03ffc842-7cf2-4733-b7c2-e263b08b62cc)
• TRAIN SIZE: Number of applicable previous games used to train model  <br>
• SPLIT DETAILS: {Tree Depth: ('Feature', Threshold value)} <br>
• X_test: [(Feature Name, Feature Value, Tree Decision)]<br>
&nbsp;&nbsp;&nbsp; F indicates less than or equal to feature value (<=) is false so final node is left side <br>
&nbsp;&nbsp;&nbsp; T indicates less than or equal to feature value (<=) is true so final node is right side <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH DET @ IND, GAMEID: 22300793 DECISION TREE PLOTS
![DET@IND_TREE](https://github.com/user-attachments/assets/f5f65895-f87b-4195-8faa-8d8905ffe56b)
<br>
• Model identifies Percent of Points (Off Turnovers) in last 3 games played (%PTS OFF TOL3MA) has lowest weighted Gini Impurity & best split for team, DET (Detroit Pistons) <br>
• Model identifies Percent of Points (2-Point Field Goals: Mid Range) in last game played (%PTS 2PT MRL1MA) has lowest weighted Gini Impurity & best split for team, IND (Indiana Pacers)
## MATCH DET @ IND, GAMEID: 22300793 WEIGHTED GINI IMPUTITIES
![detGINI](https://github.com/user-attachments/assets/77c72a5f-2350-4259-893d-2034312c572c)
![indGINI](https://github.com/user-attachments/assets/383ad320-55e3-4a74-8522-e497ebed1f4c)
<br><br>
## MATCH NYK @ PHI, GAMEID: 22300794 TRAIN & TEST DETAILS
![NYK@PHI_MATCHRESULTS](https://github.com/user-attachments/assets/99d414a6-5622-4e09-86a4-74a900ae2572)
![NYK@PHI_TESTDETAILS](https://github.com/user-attachments/assets/1336c534-1a61-46f3-8589-ac4f88fdff1b)
<br><br>
• TRAIN SIZE: Number of applicable previous games used to train model  <br>
• SPLIT DETAILS: {Tree Depth: ('Feature', Threshold value)} <br>
• X_test: [(Feature Name, Feature Value, Tree Decision)]<br>
&nbsp;&nbsp;&nbsp; F indicates less than or equal to feature value (<=) is false so final node is left side <br>
&nbsp;&nbsp;&nbsp; T indicates less than or equal to feature value (<=) is true so final node is right side <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH NYK @ PHI, GAMEID: 22300794 DECISION TREE PLOTS
![NYK@PHI_TREE](https://github.com/user-attachments/assets/62ade814-eb96-465a-9f67-d49ca3b26537)
<br>
• Model identifies Percent of Points (2-Point Field Goals) in last 5 games played (%PTS 2PTL5MA) has lowest weighted Gini Impurity & best split for team, NYK (New York Knicks) <br> 
• Model identifies Percent of Points (2-Point Field Goals) in last 2 games played (%PTS 2PTL2MA) has lowest weighted Gini Impurity & best split for team, PHI (Philadelphia 76ers)
## MATCH NYK @ PHI, GAMEID: 22300794 WEIGHTED GINI IMPUTITIES
![nykGINI](https://github.com/user-attachments/assets/7e02a2ac-f19c-40ef-9f5e-96931247b193)
![phiGINI](https://github.com/user-attachments/assets/fa9d13b1-114d-42e8-b19b-5967f4e44c0b)
<br><br>
## MATCH BKN @ TOR, GAMEID: 22300795 TRAIN & TEST DETAILS
![BKN@TOR _MATCHRESULTS](https://github.com/user-attachments/assets/d460c4e8-f0c9-4f99-b895-656048ddc009)
![BKN@TOR_TESTDETAILS](https://github.com/user-attachments/assets/e97a881a-4124-4655-8c35-c4fde63080ab)
• TRAIN SIZE: Number of applicable previous games used to train model  <br>
• SPLIT DETAILS: {Tree Depth: ('Feature', Threshold value)} <br>
• X_test: [(Feature Name, Feature Value, Tree Decision)]<br>
&nbsp;&nbsp;&nbsp; F indicates less than or equal to feature value (<=) is false so final node is left side <br>
&nbsp;&nbsp;&nbsp; T indicates less than or equal to feature value (<=) is true so final node is right side <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH BKN @ TOR, GAMEID: 22300795 DECISION TREE PLOTS
![BKN@TOR_TREE](https://github.com/user-attachments/assets/7934dab5-d6cf-4c5a-a1d9-70dc33711d27)
<br>
• Model identifies Percent of 2 Point Field Goals Made Unassisted in last 5 games played (2FGM %UASTL5MA) has lowest weighted Gini Impurity & best split for team, BKN (Brooklyn Nets) <br>
• Model identifies Percent of Points (Off Turnovers) in last 2 games played (%PTS OFF TOL2MA) has lowest weighted Gini Impurity & best split for team, TOR (Toronto Raptors)
## MATCH BKN @ TOR, GAMEID: 22300795 WEIGHTED GINI IMPUTITIES
![bknGINI](https://github.com/user-attachments/assets/2175a8ea-540f-4c4e-878c-a35738ff6eda)
![torGINI](https://github.com/user-attachments/assets/c0539cdc-5fee-43c9-80f7-35c8de685f00)
<br><br>
## MATCH PHX @ DAL, GAMEID: 22300796 TRAIN & TEST DETAILS
![PHX@DAL_MATCHRESULTS](https://github.com/user-attachments/assets/586e5238-2964-400c-bde0-a1c22ca2b065)
![PHX@DAL_TESTDETAILS](https://github.com/user-attachments/assets/ec4c8357-55d8-4eb1-86b9-6d42a82547ec)
• TRAIN SIZE: Number of applicable previous games used to train model  <br>
• SPLIT DETAILS: {Tree Depth: ('Feature', Threshold value)} <br>
• X_test: [(Feature Name, Feature Value, Tree Decision)]<br>
&nbsp;&nbsp;&nbsp; F indicates less than or equal to feature value (<=) is false so final node is left side <br>
&nbsp;&nbsp;&nbsp; T indicates less than or equal to feature value (<=) is true so final node is right side <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH PHX @ DAL, GAMEID: 22300796 DECISION TREE PLOTS
![PHX@DAL_TREE](https://github.com/user-attachments/assets/b9bf3d65-496d-4dcc-868e-e988215f44c7)
<br>
• Model identifies Percent of Points (Free Throws) in last 4 games played (%PTS FTL4MA) has lowest weighted Gini Impurity & best split for team, PHX (Phoenix Suns) <br>
• Model identifies 3 Pointers Made (Percent Assisted) in last game played (3FGM %ASTL1MA) has lowest weighted Gini Impurity & best split for team, DAL (Dallas Mavericks)
<br><br>
## MATCH PHX @ DAL, GAMEID: 22300796 WEIGHTED GINI IMPUTITIES
![phxGINI](https://github.com/user-attachments/assets/2f44a9bd-bac6-48b3-a106-6bddff8d8384)
![dalGINI](https://github.com/user-attachments/assets/675ec40a-2171-442e-9417-ccb61c939e5c)
## MATCH BOS @ CHI, GAMEID: 22300797 TRAIN & TEST DETAILS
![BOS@CHI_MATCHRESULTS](https://github.com/user-attachments/assets/60155005-ed24-405a-99b3-0b53f23c11d8)
![BOS@CHI_TESTDETAILS](https://github.com/user-attachments/assets/e39d8b28-bd76-422c-9d25-079029e609c9)
• TRAIN SIZE: Number of applicable previous games used to train model  <br>
• SPLIT DETAILS: {Tree Depth: ('Feature', Threshold value)} <br>
• X_test: [(Feature Name, Feature Value, Tree Decision)]<br>
&nbsp;&nbsp;&nbsp; F indicates less than or equal to feature value (<=) is false so final node is left side <br>
&nbsp;&nbsp;&nbsp; T indicates less than or equal to feature value (<=) is true so final node is right side <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH BOS @ CHI, GAMEID: 22300797 DECISION TREE PLOTS
![BOS@CHI_TREE](https://github.com/user-attachments/assets/a01a562f-15fe-49a5-a424-18fa75351b31)
<br>
• Model identifies Field Goals Made (Unassisted) in last 3 games played (FGM %UASTL3MA) has lowest weighted Gini Impurity & best split for team, BOS (Boston Celtics) <br>
• Model identifies %PTS FBPSL3MA in last 3 games played (%PTS FBPSL3MA) has lowest weighted Gini Impurity & best split for team, CHI (Chicago Bulls)
## MATCH BOS @ CHI, GAMEID: 22300797 WEIGHTED GINI IMPUTITIES
![bosGINI](https://github.com/user-attachments/assets/b67944bc-8342-4b60-83ee-fc85382db4ed)
![chiGINI](https://github.com/user-attachments/assets/236a9661-45e8-4ac1-9d11-250f12fdbace)
<br><br>
## MATCH HOU @ NOP, GAMEID: 22300798 TRAIN & TEST DETAILS
![HOU@NOP_MATCHRESULTS](https://github.com/user-attachments/assets/8839fe2e-ce95-4b12-ac52-de8c6919ea94)
![HOU@NOP_TESTDETAILS](https://github.com/user-attachments/assets/5af9d6bc-0212-4c45-88ca-83c05b69cab1)
• TRAIN SIZE: Number of applicable previous games used to train model  <br>
• SPLIT DETAILS: {Tree Depth: ('Feature', Threshold value)} <br>
• X_test: [(Feature Name, Feature Value, Tree Decision)]<br>
&nbsp;&nbsp;&nbsp; F indicates less than or equal to feature value (<=) is false so final node is left side <br>
&nbsp;&nbsp;&nbsp; T indicates less than or equal to feature value (<=) is true so final node is right side <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH HOU @ NOP, GAMEID: 22300798 DECISION TREE PLOTS
![HOU@NOP_TREE](https://github.com/user-attachments/assets/c429ba95-6776-4ee6-84f8-017f36ddfeec)
<br>
• Model identifies Percent of Points (3-Point Field Goals) in last 2 games played (%PTS 3PTL2MA) has lowest weighted Gini Impurity & best split for team, HOU (Houston Rockets) <br>
• Model identifies Percent of Field Goals Attempted (3 Pointers) in last 4 games played (%FGA 3PTL4MA) has lowest weighted Gini Impurity & best split for team, NOP (New Orleans Pelicans)
## MATCH HOU @ NOP, GAMEID: 22300798 WEIGHTED GINI IMPUTITIES
![houGINI](https://github.com/user-attachments/assets/cd0240d1-b41c-4e85-bf29-0f803b62cf5c)
![nopGINI](https://github.com/user-attachments/assets/3b46339d-7848-459d-819e-541d0e926de6)
<br><br>
## MATCH LAC @ OKC, GAMEID: 22300799 TRAIN & TEST DETAILS
![LAC @ OKC_MATCHRESULTS](https://github.com/user-attachments/assets/5170d9d5-ee03-470a-928f-eb332e337a9e)
![LAC @ OKC_TESTDETAILS](https://github.com/user-attachments/assets/89dd1b16-68c4-4e9c-9eae-6299fe74561c)
• TRAIN SIZE: Number of applicable previous games used to train model  <br>
• SPLIT DETAILS: {Tree Depth: ('Feature', Threshold value)} <br>
• X_test: [(Feature Name, Feature Value, Tree Decision)]<br>
&nbsp;&nbsp;&nbsp; F indicates less than or equal to feature value (<=) is false so final node is left side <br>
&nbsp;&nbsp;&nbsp; T indicates less than or equal to feature value (<=) is true so final node is right side <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH LAC @ OKC, GAMEID: 22300799 DECISION TREE PLOTS
![LAC@OKC_TREE](https://github.com/user-attachments/assets/5a8c2883-f6c0-4256-b219-38947b107550)
<br>
• Model identifies Percent of 2 Point Field Goals Made Unassisted in last 5 games played (2FGM %UASTL5MA) has lowest weighted Gini Impurity & best split for team, LAC (Los Angeles Clippers) <br>
• Model identifies Percent of Field Goals Attempted (2 Pointers) in last 2 games played (%FGA 2PTL2MA) has lowest weighted Gini Impurity & best split for team, OKC (Oklahoma City Thunder)
## MATCH LAC @ OKC, GAMEID: 22300799 WEIGHTED GINI IMPUTITIES
![lacGINI](https://github.com/user-attachments/assets/3a29b0c9-82c6-42fa-81b0-1da212fb36c5)
![okcGINI](https://github.com/user-attachments/assets/758bb3bc-6ffc-47cb-bb52-e2f60ede109d)
<br><br>
## MATCH WAS @ DEN, GAMEID: 22300800 TRAIN & TEST DETAILS
![WAS@DEN_MATCHRESULTS](https://github.com/user-attachments/assets/f2075256-06e3-4547-b71d-16b9668bffcd)
![WAS@DEN_TESTDETAILS](https://github.com/user-attachments/assets/05cbaa19-6d08-44c5-8e60-e3f9a69c68a4)
• TRAIN SIZE: Number of applicable previous games used to train model  <br>
• SPLIT DETAILS: {Tree Depth: ('Feature', Threshold value)} <br>
• X_test: [(Feature Name, Feature Value, Tree Decision)]<br>
&nbsp;&nbsp;&nbsp; F indicates less than or equal to feature value (<=) is false so final node is left side <br>
&nbsp;&nbsp;&nbsp; T indicates less than or equal to feature value (<=) is true so final node is right side <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH WAS @ DEN, GAMEID: 22300800 DECISION TREE PLOTS
![WAS@DEN_TREE](https://github.com/user-attachments/assets/eea82a7c-3045-49ab-828e-80aec9c2fecd)
<br>
• Model identifies Percent of 2 Point Field Goals Made Unassisted in last 3 games played (2FGM %UASTL3MA) has lowest weighted Gini Impurity & best split for team, WAS (Washington Wizards) <br>
• Model identifies Field Goals Made (Unassisted) in last 3 games played (FGM %UASTL3MA) has lowest weighted Gini Impurity & best split for team, DEN (Denver Nuggets)
## MATCH WAS @ DEN, GAMEID: 22300800 WEIGHTED GINI IMPUTITIES
![wasGINI](https://github.com/user-attachments/assets/902427da-047c-47bf-8cba-625dc8a1742a)
![denGINI](https://github.com/user-attachments/assets/5275bad3-e8ad-4104-986a-86dd76019e22)
<br><br>
## MATCH CHA @ UTA, GAMEID: 22300801 TRAIN & TEST DETAILS
![CHA@UTA_MATCHRESULTS](https://github.com/user-attachments/assets/04e2c954-1b00-4c1e-b7c5-0cc1714ab69e)
![CHA@UTA_TESTDETAILS](https://github.com/user-attachments/assets/6622ca1c-8fcf-46d7-b05a-36806f0b8538)
• TRAIN SIZE: Number of applicable previous games used to train model  <br>
• SPLIT DETAILS: {Tree Depth: ('Feature', Threshold value)} <br>
• X_test: [(Feature Name, Feature Value, Tree Decision)]<br>
&nbsp;&nbsp;&nbsp; F indicates less than or equal to feature value (<=) is false so final node is left side <br>
&nbsp;&nbsp;&nbsp; T indicates less than or equal to feature value (<=) is true so final node is right side <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH CHA @ UTA, GAMEID: 22300801 DECISION TREE PLOTS
![CHA@UTA_TREE](https://github.com/user-attachments/assets/ec36c0bf-29fe-4089-bf40-4d596c970bbb)
<br>
• Model identifies Percent of Points (Off Turnovers) in last 3 games played (%PTS OFF TOL3MA) has lowest weighted Gini Impurity & best split for team, CHA (Charlotte Hornets) <br>
• Model identifies Percent of Points (3-Point Field Goals) in last 5 games played (%PTS 3PTL5MA) has lowest weighted Gini Impurity & best split for team, UTA (Utah Jazz)
## MATCH CHA @ UTA, GAMEID: 22300801 WEIGHTED GINI IMPUTITIES
![chaGINI](https://github.com/user-attachments/assets/31e35d66-c03c-4619-b58f-ebfff6b433f9)
![utaGINI](https://github.com/user-attachments/assets/5b7ff624-14c3-49e5-837b-ef10531dafa3)
<br><br>
## MATCH LAL @ GSW, GAMEID: 22300802 TRAIN & TEST DETAILS
![LAL@GSW_MATCHRESULTS](https://github.com/user-attachments/assets/de9ffabf-b5a0-48d3-be4e-37da696127af)
![LAL@GSW_TESTDETAILS](https://github.com/user-attachments/assets/4bcb4e99-e29a-4137-9b18-5e1c9aac7ec0)
• TRAIN SIZE: Number of applicable previous games used to train model  <br>
• SPLIT DETAILS: {Tree Depth: ('Feature', Threshold value)} <br>
• X_test: [(Feature Name, Feature Value, Tree Decision)]<br>
&nbsp;&nbsp;&nbsp; F indicates less than or equal to feature value (<=) is false so final node is left side <br>
&nbsp;&nbsp;&nbsp; T indicates less than or equal to feature value (<=) is true so final node is right side <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH LAL @ GSW, GAMEID: 22300802 DECISION TREE PLOTS
![LAL@GSW_TREE](https://github.com/user-attachments/assets/ba8ee1d7-6304-4cb0-8e01-20a0abff97bc)
<br>
• Model identifies Percent of Field Goals Attempted in last game played (%FGA 2PTL1MA) has lowest weighted Gini Impurity & best split for team, LAL (Los Angeles Lakers) <br>
• Model identifies Percent of Points (3-Point Field Goals) in last 3 games played (%PTS 3PTL3MA) has lowest weighted Gini Impurity & best split for team, GSW (Golden State Warriors)
## MATCH LAL @ GSW, GAMEID: 22300802 WEIGHTED GINI IMPUTITIES
![lalGINI](https://github.com/user-attachments/assets/4d61b53c-2e70-4d78-8de3-5ffd712ac94e)
![gswGINI](https://github.com/user-attachments/assets/53c4aa91-4c3f-432d-9ed6-94eea8d15878)
<br><br>
## MATCH SAS @ SAC, GAMEID: 22300803 TRAIN & TEST DETAILS
![SAS@SAC_MATCHRESULTS](https://github.com/user-attachments/assets/b638954e-d1c1-42a9-9ee2-8b2176a9d8c1)
![SAS@SAC_TESTDETAILS](https://github.com/user-attachments/assets/e3ae6e72-42b7-4074-81a2-538db63707b2)
• TRAIN SIZE: Number of applicable previous games used to train model  <br>
• SPLIT DETAILS: {Tree Depth: ('Feature', Threshold value)} <br>
• X_test: [(Feature Name, Feature Value, Tree Decision)]<br>
&nbsp;&nbsp;&nbsp; F indicates less than or equal to feature value (<=) is false so final node is left side <br>
&nbsp;&nbsp;&nbsp; T indicates less than or equal to feature value (<=) is true so final node is right side <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH SAS @ SAC, GAMEID: 22300803 DECISION TREE PLOTS
![SAS@SAC_TREE](https://github.com/user-attachments/assets/db8dc9b3-5919-4127-a5cc-26a592d14dd1)
<br>
• Model identifies Percent of Field Goals Made Assisted in last 2 games played (FGM %ASTL2MA) has lowest weighted Gini Impurity & best split for team, SAS (San Antonio Spurs) <br>
• Model identifies 3 Pointers Made (Percent Assisted) in last 5 games played (3FGM %ASTL5MA) has lowest weighted Gini Impurity & best split for team, SAC (Sacramento Kings)
## MATCH SAS @ SAC, GAMEID: 22300803 WEIGHTED GINI IMPUTITIES
![sasGINI](https://github.com/user-attachments/assets/96bde20f-6f3b-42a8-a0f5-3a6d99cbd462)
![sacGINI](https://github.com/user-attachments/assets/b8dada79-d246-4a8d-98e5-a1af01f514bc)
<br><br>

# OBJECTIVES:
•	For each of the 30 NBA teams, utilize data from previous games played to calculate probability estimate of team winning their next game <br>
•	Model predictions begin on games played post the NBA 2024 All Star Game played on 2024-02-18 <br>
•	Compare model's predicted winner to 1) actual winner 2) team listed as the betting favorite <br>
•	Identify features with greatest impact on team wins <br>

# DATA SOURCES: 
<b><i>NBA.com</i></b><br>
&nbsp;&nbsp;&nbsp; [Traditional Box Score](https://www.nba.com/stats/teams/boxscores-traditional?SeasonType=Regular+Season&Season=2023-24) <br>
&nbsp;&nbsp;&nbsp; [Advanced Box Score](https://www.nba.com/stats/teams/boxscores-advanced?SeasonType=Regular+Season&Season=2023-24) <br>
&nbsp;&nbsp;&nbsp; [Four Factors  Box Score](https://www.nba.com/stats/teams/boxscores-four-factors?SeasonType=Regular+Season&Season=2023-24) <br>
&nbsp;&nbsp;&nbsp; [Misc Box Score](https://www.nba.com/stats/teams/boxscores-misc?SeasonType=Regular+Season&Season=2023-24) <br>
&nbsp;&nbsp;&nbsp; [Scoring Box Score](https://www.nba.com/stats/teams/boxscores-scoring?SeasonType=Regular+Season&Season=2023-24) <br>
&nbsp;&nbsp;&nbsp; [NBA Stats Glossary](https://www.nba.com/stats/help/glossary) <br>

<i><b>VEGASINSIDER.com</i></b><br>
&nbsp;&nbsp;&nbsp; [NBA Odds & Betting Lines](https://www.vegasinsider.com/nba/odds/las-vegas) <br>
# CONCLUSIONS:
<b>PREDICTION RESULTS BY TEAM</b>
<br>
![percentCorrect](https://github.com/user-attachments/assets/cbe06445-8df7-400a-901e-70839ace14d4)
<b><i> Model correctly predicts a league high of 100% (18-0) vs Betting Favorite for Denver Nuggets vs Betting Favorite & 100% (2-0) for Detroit Pistons vs Actual Result </i></b>
# CONCLUSIONS:
<br><br>
![numberCorrect](https://github.com/user-attachments/assets/83030189-48dd-48dc-8388-180694852426)
<b><i>Model correctly predicts a league high of 19 vs Actual Result & 24 vs Betting Favorite for Boston Celtics </i></b>
<br><br>
![numberIncorrect](https://github.com/user-attachments/assets/24363a88-79ec-41de-99c1-a049ac08faee)
<b><i>Model incorrectly predicts a league high of 9 vs Actual Result for Toronto Raptors </i></b>
# CONCLUSIONS:
<b>FEATURE IMPACT BY TEAM</b><br>
<b><i> Teams where same feature is used for each prediction are highlighted</i></b>
<br>
![dtreeMaxFeatures](https://github.com/user-attachments/assets/2ba75ed7-8610-4496-9fd2-09d5d2b36e06)
<br>
# CONCLUSIONS:
<b>How feature, FGM %UASTL3MA for Boston Celtics (BOS) compares to rest of league </b> <br>
![sameFeaturesBOS](https://github.com/user-attachments/assets/d88ef1cc-4439-4c17-a567-b23dcedcc8a9)
![BOS](https://github.com/user-attachments/assets/220ec7bc-8bb1-4241-969d-843652352678)
<br><br>
![BOSW%](https://github.com/user-attachments/assets/18392028-8e5b-4aa5-a042-f8fd8012182c)
<br>
# CONCLUSIONS:
<b>How feature, %FGA 3PTL4MA for Memphis Grizzlies (MEM) compares to rest of league </b> <br>
![sameFeaturesMEM](https://github.com/user-attachments/assets/8be5be2b-80cc-4a4a-bb6e-dd15f2eefd36)
![MEM](https://github.com/user-attachments/assets/d7694bfb-cd4a-44de-adf2-84a10dcfc865)
<br><br>
![MEMW%](https://github.com/user-attachments/assets/852f03a6-bc44-421a-adca-06c56d66d3eb)
<br>
# CONCLUSIONS:
<b>How feature, %PTS PITPL5MA for Milwaukee Bucks (MIL) compares to rest of league </b> <br>
![sameFeaturesMIL](https://github.com/user-attachments/assets/eb739b72-b272-4a8b-8b51-24ec667011c9)
![MIL](https://github.com/user-attachments/assets/7cd56386-ab20-49fe-bfa6-9deeb3d1cc01)
<br><br>
![MILW%](https://github.com/user-attachments/assets/0fd5ba64-e226-4937-8dfb-b716d86b3616)
<br>
# CONCLUSIONS:
<b>How feature, FGM %UASTL3MA for Orlando Magic (ORL) compares to rest of league </b> <br>
![sameFeaturesORL](https://github.com/user-attachments/assets/11898350-8837-4524-bce2-659ac1815d3c)
![ORL](https://github.com/user-attachments/assets/e265a981-cc5b-49ef-930e-90465dffc41e)
<br><br>
![ORLW%](https://github.com/user-attachments/assets/99bf9a9e-7c4d-45d6-834d-b6bbe0bd0f72)

![](https://komarev.com/ghpvc/?username=olutosinfashusi)
