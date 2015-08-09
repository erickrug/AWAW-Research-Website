# AWAW-Research-Website
An attempt to build a website to help users play A World At War boardgame

// AWAWResearch.js file Created 8/9/2015
//
// by Eric Krug

// The purpose of this program is to automate the "Research" portion of the game "A World at War" (AWAW)

// 1) Determine if this is a European, Pacific, or Global Game with a pop-up box

var scenario;

// 2) Determine if this is a standard AWAW game or a Gathering Storm (GS) game with a pop-up box

var GS;

// 2A) Set the initial values for a standard game (Fall 1939, RP assignments, initial reaults, BRPs, DPs allocated)

var year;
var turn;

// 2B) Input the values for a GS game

// 3) First turn / every YSS - Start the research for each faction (loop thru EuroAxis, Japan, WA, Russia)

// 3A) Determine the number of RPs and the limits for each category of research (Rules section 41.3)
//    i) Catgegory - no more than 1/2 
//    ii) Project - between 3 and 6
//    iii) Hi tech - start at one, increment by one per year
//    iv) Dates - as shown in rules
//    v) Production - no limits on RP allocation, but are limits on usage 
//    vi) need to input USAT and USJT levels to determine RPs

/* 41.2 RESEARCH POINTS (RPs):
41.21 BASIC RP ALLOTMENTS: The basic allotment of RPs for each major power is:
A. GERMANY: 8.
B. ITALY: 2.
C. JAPAN: 6.
D. RUSSIA: 6.
E. BRITAIN: 6.
F. FRANCE: 3.
G. U.S.: 10 (once the U.S. is at war with both Germany and Japan).
41.211 AMERICAN RPs PRIOR TO ENTRY: During each YSS before it enters the war, the U.S. receives one RP for every ten USAT and USJT levels
 (combine both tension levels and round down). The effective tension levels for the winter turn are used.
EXAMPLE: At the end of 1941, the U.S. is at war with Japan and the effective USAT level is 39. In the 1942 YSS, the U.S. receives five RPs
 for the Pacific and three RPs for Europe, in addition to the RPs it receives for its BRPs and BRP growth.
41.212 CHINA: China never receives RPs, does not conduct research and may not use RPs for production.
41.22 ADDITIONAL RPs FROM BRP LEVELS: In addition to its basic RP allotment, in each YSS (but not during the opening setup of the Campaign
 game and 1939 scenarios) each major power receives one RP for every 50 BRPs in its BRP total.
41.221 AMERICAN RPs IN A EUROPEAN SCENARIO: In a European scenario, the U.S. receives one additional RP in the 1941 YSS, three additional 
RPs in the 1942 YSS, and five additional RPs in the 1943 and each subsequent YSS, to reflect RPs from the Pacific.
41.23 ADDITIONAL RPs FROM BRP GROWTH: Each major power receives one additional RP for every 25 BRPs of growth (round down) in each YSS. 
This additional RP is received for that year only and is based on BRP growth only for that year. The BRP growth itself is unaffected. 
Increases in the BRP value of Russian ICs and base increases from mobilizations (36.21) are not counted.
41.24 USE OF DPs AS RPs FOR INTELLIGENCE: The intelligence category as a whole is considered an eligible project for DP allocation. DPs 
allocated to intelligence act as RPs. A player may therefore allocate up to half his RPs (41.31A) and one-third of his DPs (49.31) to 
intelligence. The limit on the number of points (the total of RPs and DPs) allocated to each intelligence project, including general 
research, still applies (41.31B).
41.25 ADDITIONAL JAPANESE RPs FOR INTELLIGENCE: In addition to its normal RP allotment, during the 1939 opening setup and in each subsequent
 YSS Japan receives one additional RP which may only be allocated to intelligence projects. This RP is not taken into account in determining
 the number of Japanese RPs which may be assigned to other research categories (41.31A). */

// 3B) Allow assignment of RPs for each category, add code names

// 4) Iterate thru turns for each faction (EuroAxis, Japan, WA, Russia)

// 4A) Query about active spy rings / use of counterintels to kill them

// 4B) Allow player to select and roll dice for each category (all five in most cases)
//    i) Roll dice, select middle, if 1 or 2 allow re-assignemnt of RPs, zero out RPs or reduce in those categories
//    ii) determine new modifiers, breakthroughs, and failures - include negative mods for BTs
//    iii) update displays

// 4C) Query about activating production, display costs (modified by General Research), reduce RPs accordingly

// 4D) If end of winter, increment year and do step 3, otherwise, increment turn and redo step 4

// Need data structures for info
// Need procedures to implement above
