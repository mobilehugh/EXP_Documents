::: mermaid
graph LR;
%% ROLLS
    ROLLS-->Target;
    ROLLS-->Challenge;
    ROLLS-->Generative;
    ROLLS-->Jelly

%% TARGET, CHALLENGE, GENERATIVE, JELLY
    Target-->Attack[Attack Roll]
    Target-->Task[Task Roll]
    Target-->Drive[Driving Roll]
    Target-->DSS
    Target-->REC

    Challenge-->Saves
    Challenge-->Initiative
    Challenge-->Ambush
    Challenge-->Att_Chall[Attribute]
    Challenge-->Sphincter

    Generative-->Incentivized
    Generative-->Chance

    Jelly-->Chocolate
    Jelly-->Jam
    Jelly-->Chicken

%% INCENTIVIZED, CHANCE, 

    Incentivized-->Damage
    Incentivized-->Attibutes
    Incentivized-->Quantities

    Chance-->TOYs
    Chance-->Mutations
    Chance-->Descriptions
    Chance-->Abilities


%% CHECKS
    Attack[Attack Roll]-.-Checks
    Task[Task Roll]-.-Checks
    Drive[Driving Roll]-.-Checks
    DSS-.-Checks
    REC-.-Checks
    Saves-.-Checks

%% CHALLENGERS
    Initiative-.->order[All Personas, ranked]
    Ambush-.->surprise[All Personas, listed]
    Att_Chall[Attribute]<-.->fight[Persona vs Persona]
    Sphincter<-.->PVR[Player vs Referee]

%% FLAVOUR FLAVs
    Chocolate-->Sweet
    Jam-->Sweeter
    Chicken-->Savoury

%% CHECKERY CHECKS
    Checks-. Attack Roll .->CH[Critical Hit]
    Checks-. Attack Roll .->CM[Critical Miss]
    Checks-. Weapon .->Malfunction
    Checks-. Task Roll .->OW[Otto Win]
    Checks-. Task Roll .->OF[Otto Fail]

:::