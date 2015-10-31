---
layout: page
title: "Site Generator"
date: 2005-05-01T18:53:33+00:00
comments: true
sharing: true
footer: true
group: Mechanics
---

PLANET GENERATION SYSTEM
------------------------

Version 2.0 (4-Dec-95)
Copyright 1995 by Ross Smith %3calien@netlink.co.nz>



## INTRODUCTION

This is a reasonably quick and simple system for generating complete planetary systems in rough detail, and the most interesting planets in somewhat greater detail. It also includes a system for generating intelligent life forms. It isn't tied to any particular game mechanics, and should be usable with any SFRP system.

I designed it because I've never been very impressed by the planet generation schemes in most SF role-playing games, which are usually either too unrealistic or too complicated (or, frequently, both). I wanted a scheme that was simple enough to generate systems fairly quickly, while still being designed by someone who knew one end of a Hertzsprung-Russell diagram from the other (hint: neither end is likely to have anything resembling Earth orbiting it).

You will need some six-sided and ten-sided or twenty-sided dice (or, of course, a computer with a good random number function). I assume you're familiar with the usual dice notation (so you know what something like "2D6+3" means). This system requires rolls on D6, D10, D20, and D100.  Unless otherwise stated, all results of less than zero should be counted as zero, and all fractional results should be rounded to the nearest whole number (round halves upwards).

<div class='bs-callout bs-callout-info'>
This file is copyright 1995 by Ross Smith. It may be distributed and archived freely, provided no changes are made. Comments can be mailed to me at the address above, or posted to rec.games.frp.misc.
</div>

### Version history:

1.0 (1-Aug-93): Original version.

1.1 (2-Oct-93): Expanded star type table; orbit periods added; various
minor changes.

1.2 (30-Oct-94): Minor revisions.

2.0 (4-Dec-95): Minor revisions to star and planet system; added sections
on colonisation and intelligent life.


## STAR SYSTEMS


In the local region of the Galaxy, there is about one star system per 600 cubic light-years. I suggest using cube-shaped sectors either 25 or 50 light-years on a side. A 25 light-year sector has 8D6-2 star systems (average 26); a 50 light-year sector has 6D20+145 systems (average 208; more appropriate to generation by a computer program than by hand). Place the systems at random within the sector (roll D100/4 or D100/2 for each of the X, Y, and Z coordinates).

To find the number of stars in a system, roll D100 on the following table:

    D100   Stars
    -----  -----
    1-40   1
    41-90  2
    91-99  3
    100    4

Stars are classified into seven "spectral types", based on their temperature and colour. The types are O (blue), B (blue-white), A (white), F (yellow-white), G (yellow), K (orange), and M (red); astronomers use the mnemonic "Oh, Be A Fine Girl, Kiss Me" to remember the sequence. The seven types are each divided into ten subclasses, indicated by a digit from 0 to 9 after the spectral type (except type O, which is normally divided only into subclasses 5 to 9). The Sun, for example, is type G2.

A Hertzsprung-Russell diagram is a plot of stars with spectral type on the horizontal axis and luminosity on the vertical axis. The majority of stars fall into the "main sequence", which runs roughly diagonally, from bright, blue-white O-type stars at the top left of the diagram to dim M-type red dwarfs at the bottom right, with yellow dwarfs like the Sun falling almost exactly in the middle. Other types of stars are above or below the main sequence.

Red giants (indicated by a "g" prefix on the spectral type, e.g. "gM5") and supergiants (indicated by a "c" prefix, e.g. "cK0") are late stages in the life cycle of massive stars. White dwarfs (indicated by a "D" prefix, e.g.  "DA"), much dimmer than most main sequence stars, are the final stage in the evolution of most stars. The most massive stars will end up as neutron stars or black holes (these have no spectral types; the tables below use "NS" and "BH" to represent them).

For each star in a system, roll D100 (one to three times) on the following table, to get the general description and the specific spectral class of the star. A subclass number should also be generated for main sequence and giant stars (white dwarfs are not usually given a subclass).  The stars in a system should be listed in descending order of luminosity.  Take the basic groups in order (supergiants, giants, main sequence, white dwarfs, neutron stars, black holes); within each group, list stars in order of spectral type.

    First  Second  Third   Basic          Spectral  Subclass
    D100   D100    D100    type           class
    -----  ------  ------  -------------  --------  ---------
    1      1       1-10    Supergiant     cB        D10-1
    ...    ...     11-20   ...            cA        D10-1
    ...    ...     21-40   ...            cF        D10-1
    ...    ...     41-60   ...            cG        D10-1
    ...    ...     61-80   ...            cK        D10-1
    ...    ...     81-100  ...            cM        D10-1
    ...    2-5     --      Giant          gF        D10-1
    ...    6-10    --      ...            gG        D10-1
    ...    11-55   --      ...            gK        D10-1
    ...    56-95   --      ...            gM        D10-1
    ...    96-99   --      Neutron star   NS        --
    ...    100     1-20    Black hole     BH        --
    ...    ...     21-100  Main sequence  O         (D10/2)+4
    2      --      --      ...            B         D10-1
    3-4    --      --      ...            A         D10-1
    5-8    --      --      ...            F         D10-1
    9-15   --      --      ...            G         D10-1
    16-30  --      --      ...            K         D10-1
    31-93  --      --      ...            M         D10-1
    94     --      --      White dwarf    DB        --
    95-96  --      --      ...            DA        --
    97-98  --      --      ...            DF        --
    99     --      --      ...            DG        --
    100    --      --      ...            DK        --

Many astronomical references use a more detailed system of "luminosity classes", which run from I (supergiants) to VII (white dwarfs). This level of detail is probably unnecessary for gaming. If you're using a star catalogue that uses this system, you can convert the full luminosity classes to the broad classes I've used here using the following table.

    Luminosity class               Description
    -----------------------------  -------------
    I                              Supergiant
    O-A II, F II-III, G-M II-IV    Giant
    O-A III-VI, F IV-VI, G-M V-VI  Main sequence
    VII                            White dwarf


## PLANETARY SYSTEMS

Refer to the following table to generate the number of planets for each star. First determine whether there are any planets; for multiple star systems, roll only once for the whole system, using the spectral type of the primary star. If the result is affirmative, generate the number of planets for each star, based on the star's own spectral type.

    Star                     Spectral  Probability  Number of
    type                     class     of planets   planets
    -----------------------  --------  -----------  ---------
    Giant/supergiant         All       10%25          D6
    Main sequence            O-B       10%25          D10
    ...                      A         50%25          D10
    ...                      F-G       99%25          2D6+3
    ...                      K         99%25          2D6
    ...                      M         50%25          D6
    White dwarf              All       10%25          D6/2
    Neutron star/black hole  All       5%25           D6/2

Planetary systems are divided into three zones; different types of planet will tend to form in each zone. Zone A is the inner or hot zone; zone B is the intermediate or life zone; and zone C is the outer or cold zone (in our system, Mercury and Venus are in zone A, Earth and Mars are in zone B, and the asteroids and outer planets are in zone C). The following table indicates which planets are in each zone for main sequence, giant, and supergiant stars; all planets of white dwarfs, neutron stars, and black holes are considered to be in zone C.

    Total    Planets in   Planets in   Planets in
    planets  zone A       zone B       zone C
    -------  -----------  -----------  ----------
    1-3      --           Planet 1     Planets 2+
    4-5      Planet 1     Planet 2     Planets 3+
    6-7      Planet 1     Planets 2-3  Planets 4+
    8+       Planets 1-2  Planets 3-4  Planets 5+

At this point, if the star is a member of a multiple system, remove the outermost D6+1 planets (this may leave the star with no planets). Determine the planetary zones before deleting planets.

For each planet, three parameters are determined: type, size, and number of moons. Roll D100 and refer to the following table for planet type, then generate the size and moons.

    Planet         D100                    Diameter      Number
    type           Zone A  Zone B  Zone C  (km)          of moons
    -------------  ------  ------  ------  ------------  --------
    Asteroids      1-5     1-5     1-5     --            --
    Giant          --      6-8     6-75    3D6x10000     2D10
    Rock           6-60    9-40    76-80   D10x1000      D6xD6/10
    Cold           --      --      81-90   D10x1000      D6xD6/10
    Desert         61-70   41-60   91-95   (2D6+2)x1000  `D6xD6/10
    Hostile [*1]   71-100  61-80   96-100  (3D6+1)x1000  `D6xD6/10
    Marginal [*2]  --      81-90   --      (2D6+5)x1000  `D6xD6/10
    Earthlike [*2] --      91-100  --      (2D6+5)x1000  `D6xD6/10

    [*1: Count as "cold" if the star is a white dwarf, neutron star, or
    black hole.]

    [*2: Count as "hostile" if the star is anything other than a main
    sequence star of type F, G, or K.]

Asteroids: A collection of rocks that never combined to form a planet.  Usually there will be a handful of large asteroids a few hundred kilometres across, and a vast number of smaller objects.

Giant: A huge planet consisting mainly of hydrogen, ranging from ten to a thousand times the Earth's mass. Example: Jupiter.

Rock: A small, rocky planet with no atmosphere. Example: Mercury.

Cold: A small planet with no atmosphere, composed mainly of ice; found only in the outer part of a system. Example: Pluto.

Desert: Comparable in size to Earth, but with a barren surface and a thin, inert atmosphere. Example: Mars.

Hostile: Comparable in size to Earth, with an atmosphere containing no (or a negligible amount of) oxygen, but possibly with some other active component. Hostile planets may occasionally have native life forms, but they will be based on a very non-Earthlike biochemistry. Example: Venus.

Marginal: Almost Earthlike, with oxygen in the atmosphere, but with some serious problem that makes it an unpleasant place to live, such as very high or low temperature, atmospheric pressure, or oxygen level; traces of some toxic gas in the atmosphere; dangerous volcanic activity; or high radiation level. No examples in our solar system.

Earthlike: Oxygen atmosphere, temperatures not too far outside the human comfort zone, and a reasonably stable surface. Note that the presence of oxygen in the atmosphere necessarily implies the presence of life (oxygen is too reactive to occur in large amounts from geological processes alone, and would disappear in a relatively short time if life were to become extinct). Example: Earth.

The details of a system's planets can be conveniently written using the initial letter of the planet type, the size in thousands of kilometres, and a dot followed by the number of moons, if any. Asteroid belts are simply indicated by an "A" with no numbers (and are not counted towards the "official" number of planets). Use slashes to mark the zone boundaries.  Here are some examples, using our solar system and an imaginary one
generated for Alpha Centauri.

Sun
    G2, 9 planets: R5 H12 / E13.1 D7.2 / A G143.16 G121.18 G51.15 G51.8 C2.1

Alpha Centauri
    A: G2, 6 planets: R9.3 H8 / H10 M15.2 / C5.1 G110.9
    B: K0, 2 planets: R10.2 / H8 /
    C: M5, 1 planet: H17.1 / /


## EARTHLIKE AND MARGINAL PLANETS

### PHYSICAL DETAILS

Generate a planet's orbit period using the table below, dependent on the spectral type of its sun. If there are two Earthlike or marginal planets orbiting the same star, generate two periods and assign them in the correct order (the inner planet, obviously, gets the shorter period). If the outer period is less than 25%25 more than the inner one, generate both of them again.

    Star type  Orbit period
               (Earth days)
    ---------  -------------
    F0-F4      (2D100x3)+600
    F5-F9      (2D100x2)+400
    G0-G4      2D100+270
    G5-G9      2D100+150
    K0-K4      D100+120
    K5-K9      D100+70

To find the planet's rotation period, roll D100, add 10 for each moon, add 10 if the planet orbits a K-type star, and refer to the following table.

    Result   Rotation
    -------  ------------
    1-65     D20+9 hours
    66-90    D20+20 hours
    91-98    D10 days
    99-103   D100 days
    104-150  D10 days

Roll D6/2+3 (keep fractions, don't round) for the planet's density in grams per cubic centimetre. Multiply diameter by density and divide by 70000 to calculate the surface gravity in Earth gravities (round to the nearest 0.1).

Roll 2D6-4 for Earthlike planets, or D10+D6-6 for marginal planets, and multiply by 5 to find the average surface temperature in degrees Celsius (negative numbers should be retained here, not counted as zero). If a star has two planets in zone B and both of them are Earthlike or marginal, make sure the temperatures are in the right order; the outer planet should have a temperature no higher than the inner one (greenhouse effects and similar phenomena can affect a planet's temperature, but not by all that much on a planet with an approximately Earthlike atmosphere). If the outer planet's temperature comes out higher, either swap them around (if the planets are both Earthlike or both marginal) or generate both temperatures again (if there is one of each).

Use the following table to determine the proportion of the planet's surface covered by dry land, water, and ice. Roll dice for the water and ice areas (count less than zero as zero, more than 100%25 as 100%25); the land area is whatever remains. If the water and ice areas add up to more than 100%25, roll both again.

    Average       Water        Ice
    temperature   area         area
    ------------  -----------  ------------
    -20 to -10 C  (D10-5)x5 %25  (D10+10)x5 %25
    -5 to 5 C     (D20-5)x5 %25  D10x5 %25
    10 to 20 C    (5D6-8)x5 %25  (D6-2)x5 %25
    25 to 35 C    (5D6-8)x5 %25  (D6-3)x5 %25
    40 to 50 C    (5D6-8)x5 %25  (D6-4)x5 %25

If the land and water percentages are both greater than zero, the oceans are assumed to be salt water (unless the planet has the "freshwater oceans" special feature; see below). If the land percentage is zero, any oceans will be fresh water (salt reaches the ocean through runoff from the land; if there's no land, there's no salt).  A planet's mineral resources are measured on an arbitrary scale, running from 1 (worst) to 100 (best). The Earth is rated 80, fairly high, because of its high density (implying a relatively high ratio of metal to rock), and its active volcanic and tectonic processes (which carry minerals from deep in the interior to the surface). A planet's mineral resources rating is generated by the formula:

    Minerals = (Diameter / 500) + (Density x 10) + (D100 / 2) - 45


### BIOLOGICAL DETAILS

Roll D100 on each of the following tables to determine the evolutionary level of the local life forms, and their chemical basis.

    D100                  Level of development
    Earthlike  Marginal
    ---------  ---------  --------------------------------------------------
    --         1          No life
    1-10       2-30       I: Single-celled organisms only
    11-20      31-45      II: Simple invertebrates and plants (in seas)
    21-30      46-60      III: Advanced invertebrates and plants (on land)
    31-40      61-75      IV: Simple vertebrates (fish, amphibians)
    41-100     76-100     V: Advanced vertebrates (reptiles, birds, mammals)

If you get the "No life" result, life must have become extinct fairly recently by geological standards, or the oxygen in the atmosphere would have combined with surface materials and disappeared (it's difficult to say how long this would take -- perhaps a few million years). The extinction was probably caused by nuclear war or an astronomical disaster such as an asteroid strike or a nearby supernova.

    D100                 Biochemistry
    Earthlike  Marginal
    ---------  --------  ----------------
    1-20       1-5       Earthlike
    21-80      6-60      Protein-based
    81-100     61-99     Carbon-based
    --         100       Non-carbon-based

For simplicity, the many possible varieties of biochemistry are divided into four broad classes.

Earthlike: Essentially the same chemical basis as Earth's life forms, with only small differences, if any. Plants and animals with Earthlike biochemistry can often be safely eaten by humans (and vice versa).

Protein-based: Similar to Earth life in its basic chemical components, but with enough differences to make the biochemistries incompatible. Life of this type will nearly always be inedible, and frequently poisonous, to humans.

Carbon-based: Based on the same elements as Earth life, but arranged in very different compounds. Always inedible, and usually extremely poisonous.

Non-carbon-based: Completely different to Earth's biochemistry in every way. Invariably poisonous. Very rare, at least on anything resembling an Earthlike planet.


### SPECIAL FEATURES

There is no such thing as a typical Earthlike planet; every world is unique. To reflect this, some Earthlike or marginal planets will have one or more "special features" that are not covered by the usual planetary parameters. Roll a D100 three times on the following table to determine what the features are. If you get the same result (other than "No special feature") twice, roll again.

Most features are restricted to planets with certain properties (for example, the "Freshwater oceans" feature obviously requires an ocean percentage greater than zero), or are incompatible with certain other features (for example, a planet can't have both "High inclination" and "No seasons"). Some features are sufficiently hazardous to human health that they are restricted to marginal planets. See the detailed descriptions below for explanations of the incompatibilities and prerequisites. If you get an result incompatible with what you already know about the planet, roll again.

    D100    Special feature
    ------  -------------------------
            Astronomical features
    1           Eccentric orbit
    2           High inclination
    3           High tides
    4           Meteor storms
    5           No seasons
    6           Rings
            Geological features
    7           Radiation hazard
    8           Rugged terrain
    9           Volcanic activity
            Hydrographic features
    10          Freshwater oceans
    11          Many islands
    12          Poisonous oceans
    13          Swampy surface
            Atmospheric features
    14          Cloud cover
    15          Toxic gas
    16          Unstable climate
    17          Very dense atmosphere
    18          Very thin atmosphere
            Biological features
    19          Intelligent life
    20          Semi-intelligent life
    21          World forest
            Archaeological features
    22          Ancient artifacts
    23-100  No special feature


ASTRONOMICAL FEATURES

Eccentric orbit: The planet's orbit is highly elliptical, producing extremes of temperature at closest approach (periastron) and furthest distance (apastron). Incompatible with "No seasons".

High inclination: The planet's axis is tilted by more than 45 degrees, producing extreme temperature differences between summer and winter.  Incompatible with "No seasons".

High tides: A large, close moon or sun produces extremely high tides.  Requires either a K-type sun or at least one moon, and both land and water areas to be non-zero.

Meteor storms: The planet suffers frequent meteor storms, often including large asteroid or comet impacts, making the planet's surface a dangerous place. Marginal planets only.

No seasons: The planet has close to zero axial inclination and orbital eccentricity, so there are no seasonal effects. Requires a single star; incompatible with "Eccentric orbit" or "High inclination".

Rings: The planet has a natural ring system.


GEOLOGICAL FEATURES

Radiation hazard: Radioactive minerals, or fallout from a nuclear war, create a significant radiation hazard over large parts of the planet.  Marginal planets only.

Rugged terrain: The planet's land surface is almost entirely covered with mountains and rough, rocky terrain, with practically no flat plains or rounded hills. Requires a non-zero land area; incompatible with "Swampy surface".

Volcanic activity: The planet has many active volcanos, enough to make life dangerous over a large part of its surface. Marginal planets only.


HYDROGRAPHIC FEATURES

Freshwater oceans: The planet's oceans have very little salt in them, either because they're geologically young or because some life form has affected their composition. Requires both the land and water areas to be non-zero. If the land area is zero and the water area is non-zero, this feature is automatically present, independently of the special feature rolls.

Many islands: The planet's land surface is broken up into a large number of small islands, with no large continents. Requires both the land and water areas to be non-zero.

Poisonous oceans: The oceans contain some contaminant or (more likely) life form that makes the planet's sea water (and probably some of its fresh water) poisonous to humans. Marginal planets only; requires a non-zero ocean area.

Swampy surface: Most of the planet's land surface is low-lying and covered with swamps, marshes, mud, quicksand, and so on. Requires a non-zero land area; incompatible with "Rugged terrain".


ATMOSPHERIC FEATURES

Cloud cover: The planet has a permanent cloud cover over its entire surface; it probably rains most of the time. Requires a temperature greater than zero; incompatible with "Very thin atmosphere".

Toxic gas: The atmosphere contains some gas which is poisonous to humans, making filter masks necessary. Marginal planets only.

Unstable climate: The climate undergoes severe and unpredictable changes from year to year.

Very dense atmosphere: The atmosphere is dense enough to be unbreathable without special respirator equipment, except perhaps on very high mountains. Marginal planets only; incompatible with "Very thin atmosphere".

Very thin atmosphere: The atmosphere is too thin to breathe without special respirator equipment, except perhaps in very deep valleys. Marginal planets only; incompatible with "Cloud cover" or "Very dense atmosphere".


BIOLOGICAL FEATURES

Intelligent life: The planet has a native sentient life form, which may or may not have advanced technology. Requires at least level III life; incompatible with "Semi-intelligent life". Less likely with life below level V (25%25 chance, otherwise roll again).

Semi-intelligent life: The planet has a native life form which is not fully sentient yet, but comes close, and may develop further. Requires at least level III life; incompatible with "Intelligent life". Less likely with life below level V (25%25 chance, otherwise roll again).

World forest: The entire land surface (except ice caps, probably) is covered by a single huge forest. Requires a non-zero land area, and at least level II life.


ARCHAEOLOGICAL FEATURES

Ancient artifacts: Artifacts left behind by aliens, thousands or millions of years ago, exist on the planet. The aliens may or may not have been natives.


### EXAMPLES

Sun
    G2, 9 planets: R5 H12 / E13.1 D7.2 / A G143.16 G121.18 G51.15 G51.8 C2.1
    3. Earth: Earthlike, diameter 13000 km, density 5.5 g/cm3, gravity 1.0
        G, rotation 24 h, orbit period 365 d (365 local days), temperature
        15 C, surface 25%25 L 70%25 W 5%25 I, minerals 80, 1 moon, advanced
        vertebrates, Earthlike biochemistry; intelligent life

Alpha Centauri
    A: G2, 6 planets: R9.3 H8 / H10 M15.2 / C5.1 G110.9
    A4: Marginal, diameter 15000 km, density 5.0 g/cm3, gravity 1.1 G,
        rotation 8 d, orbit period 324 d (40.5 local days), temperature -5
        C, surface 35%25 L 35%25 W 30%25 I, minerals 64, 2 moons, advanced
        invertebrates, protein-based biochemistry; eccentric orbit,
        volcanic activity
    B: K0, 2 planets: R10.2 / H8 /
    C: M5, 1 planet: H17.1 / /


## COLONISATION

### SECTOR CHARACTERISTICS

Two characteristics need to be determined for an entire sector. First, decide how "civilised" the sector is -- that is, how much contact it has had with interstellar society in general, and how much development has been done. Second, choose the "opening date" for the sector -- the date at which colonisation of the sector began.

Ideally, these should be decided before you start, rather than generated at random. The following table is a suggestion for those who want one.

    D100    Sector description  Initial colonisation
    ------  ------------------  ----------------------
    1-30    Unexplored          D6x50 years ago
    31-60   Frontier            2D6x50 years ago
    61-90   Typical             (2D6x50)+250 years ago
    91-100  Developed           (2D6x50)+500 years ago

### PLANET QUALITY

Habitable (Earthlike or marginal) planets can be rated according to their desirability for human colonisation. Of course, aliens may have different criteria; if your universe includes many alien colonies, you may have to modify these rules.

Planet quality (PQ) ranges from 1 to 99 for habitable planets (a planet rated 0 would be uninhabitable, and 100 is excluded on the reasonable assumption that nothing is perfect). Start with a base value of 50, and modify as described below. If the final result is less than 1, record it as 1; if it's more than 99, record it as 99.

    Planet details                          PQ modifier
    --------------------------------------  ----------------------
    Planet type
        Earthlike                           +35
        Marginal                            0
    Rotation period
        Up to 2 days                        0
        Greater than 2 days, up to 7 days   -5
        Greater than 7 days                 -10
    Surface gravity
        Up to 1 G                           0
        Over 1 G                            -5 per 0.1 G over 1
    Surface temperature
        Below 10 degrees                    -1 per degree below 10
        10 to 30 degrees                    0
        Over 30 degrees                     -1 per degree over 30
    Land area
        Zero                                -20
        5%25 to 10%25                           -5
        15%25 to 85%25                          0
        90%25 to 95%25                          -5
        100%25                                -10
    Mineral resources                       +MR/4
    Life development
        No life                             -20
        I: Single-celled organisms          -15
        II: Simple invertebrates/plants     -10
        III: Advanced invertebrates/plants  -5
        IV: Simple vertebrates              0
        V: Advanced vertebrates             0
    Biochemistry
        Earthlike                           0
        Protein-based                       -10
        Carbon-based                        -30
        Non-carbon-based                    -50
    Special features
        Astronomical features
            Eccentric orbit                 -10
            High inclination                -5
            High tides                      -5
            Meteor storms                   -20
            No seasons                      0
            Rings                           0
        Geological features
            Radiation hazard                -30
            Rugged terrain                  -5
            Volcanic activity               -20
        Hydrographic features
            Freshwater oceans               0
            Many islands                    0
            Poisonous oceans                -30
            Swampy surface                  -10
        Atmospheric features
            Cloud cover                     -10
            Toxic gas                       -30
            Unstable climate                -5
            Very dense atmosphere           -30
            Very thin atmosphere            -30
        Biological features
            Intelligent life [*1]           0
            Semi-intelligent life [*1]      0
            World forest                    0
        Archaeological features
            Ancient artifacts               +10

    [*1: Depending on what sort of interstellar society your universe has,
    you may decide that the presence of intelligent or semi-intelligent
    life would place a world off limits to colonisation.]

(For the statistically minded, to save you some calculations: Earthlike planets average 74, with standard deviation 15; marginal planets average 24, s.d. 18.)


### COLONIES

The basic chance that a planet will be colonised depends on the sector civilisation level:

    Sector type  Colonisation chance
    -----------  ------------------------
    Unexplored   PQ / 2 percent
    Frontier     PQ percent
    Typical      PQ + 25 percent (max 99)
    Developed    PQ + 50 percent (max 99)

Roll the percentage or less on a D100. If the result is a success, find the date of colonisation:

    Colonisation date = Sector opening date + (100 - PQ) x D100 / 10

If the planet failed the original colonisation roll, or the date is later than the present date of your campaign, then the planet is uninhabited, and you can stop here.

Find out how much contact the planet has had with interstellar civilisation since its establishment. Again, the following is just a suggestion, and should be adjusted to suit your universe's historical background. The same contact level should probably be used for all inhabited planets in a system.

    Sector type  Die roll
    -----------  --------
    Unexplored   D6-3
    Frontier     D6-1
    Typical      D10
    Developed    D6+4

    Result  Contact level       Population modifier
    ------  ------------------  -------------------
    0       No contact          -6
    1-3     Occasional contact  -2
    4-7     Regular contact     0
    8-10    Extensive contact   +2

Now determine the current population and technology level of the colony.  The population level is given by:

    Colony age     Basic population roll
    -------------  ---------------------
    0-99 years     2D6 + (PQ / 20)
    100-299 years  3D6 + (PQ / 20)
    300-499 years  4D6 + (PQ / 20)
    500-999 years  5D6 + (PQ / 20)
    1000+ years    6D6 + (PQ / 20)

Adjust for the contact level, and use the following table to generate the actual population and tech level. See section 6 for a more detailed explanation of the technology levels.

    Result  Population         Tech level roll
                               No contact  Any contact
    ------  -----------------  ----------  -----------
    0-4     D100               2D6         3D6
    5-7     D100x10            2D6         3D6
    8-10    D100x100           2D6         3D6
    11-13   D100 thousand      2D6         3D6
    14-16   D100x10 thousand   2D6         3D6
    17-19   D100x100 thousand  2D6+1       3D6+1
    20-22   D100 million       2D6+2       3D6+2
    23-25   D100x10 million    2D6+3       3D6+3
    26-31   D100x100 million   2D6+4       3D6+4
    32+     D100x1000 million  2D6+5       3D6+5

    TL roll  Tech level
    -------  --------------------------
    2        I: Stone age
    3        IIa: Bronze age
    4        IIb: Classical/mediaeval
    5        IIc: Renaissance
    6        IIIa: Steam age
    7        IIIb: Twentieth century
    8-9      IIIc: Cyberpunk
    10-12    IVa: STL interstellar
    13-16    IVb: FTL interstellar
    17+      IVc: Advanced interstellar


### EXAMPLES

RGFM sector, in which these systems lie, has a typical civilisation level, and was first colonised in the year 2500 AD; the present year is 3000 AD.

System RGFM-29
    A: K2, 7 planets: H9 R9 / M9.2 H11.2 / G150.11 G130.9 G170.19
    A3. Noviy Siberia: Marginal, diameter 11000 km, density 3.5 g/cm3,
        gravity 0.6 G, rotation 2 d, orbit period 213 d (107 local days),
        temperature 0 C, surface 50%25 L 25%25 W 25%25 I, minerals 57, 2 moons,
        advanced vertebrates, protein-based biochemistry; world forest;
        planet quality 44, colonised 2657 AD, occasional contact,
        population 7800, tech level IVa (STL interstellar)
    B: K5, 1 planet: R1.1 / /

System RGFM-158
    Star: F8, 14 planets: H10.2 R7.1 / R3.3 E14 / G140.11 G110.19 C8.1
        G120.3 G140.11 R5.4 G80.8 G140.13 G120.6 G80.6
    4. Tsarina: Earthlike, diameter 14000 km, density 3.5 g/cm3, gravity
        0.7 G, rotation 29 h, orbit period 534 d (442 local days),
        temperature 5 C, surface 20%25 L 55%25 W 25%25 I, minerals 51, no moons,
        advanced vertebrates, Earthlike biochemistry; high inclination,
        rings; planet quality 83, colonised 2611 AD, regular contact,
        population 72 million, tech level IVb (FTL interstellar)


## TECHNOLOGY

This is a brief description of the tech level scale I've used. Some very approximate equivalents are given for two well-known SFRPG tech level scales, from SJG's _GURPS_ and GDW's _Traveller_.

Obviously any dates beyond the end of the twentieth century represent little more than wild guesswork. Even if you use my technology scale, you may want to change the dates and descriptions for the levels beyond present-day technology. In particular, the point at which FTL travel is developed will affect the history of your universe deeply.

Note that, in the interests of making this system usable with the vast majority of SF universes, I haven't made any allowance for the possibility that FTL travel really is impossible...

    "It can't be done!" they said to him
    And so he set to do it
    He tried to do what "couldn't be done"
    And he couldn't bloody do it.
        -- Anonymous

Group I -- Hunter-gatherer technology
    I: Stone age, before about 8000 BC [GURPS 0; Traveller 0]
        Stone tools, fire, language, spear, bow and arrow, boats
Group II -- Agricultural technology
    IIa: Bronze age, circa 8000 to 1000 BC [GURPS 1; Traveller 1 (early)]
        Copper, bronze, agriculture, wheels, swords, domestic animals,
        money, writing, sailboats, megalithic structures
    IIb: Classical/mediaeval, circa 1000 BC to 1400 AD [GURPS 2-3;
    Traveller 1 (late)]
        Iron, steel, glass, concrete, water wheel, catapult, crossbow,
        armour
    IIc: Renaissance, circa 1400 to 1700 AD [GURPS 4; Traveller 2]
        Gunpowder, printing, clockwork, telescope, large sailing ships,
        muskets, cannon
Group III -- Industrial technology
    IIIa: Steam age, circa 1700 to 1900 AD [GURPS 5; Traveller 3]
        Railways, steamships, telegraph, photography, rifles
    IIIb: Twentieth century, circa 1900 to 2000 AD [GURPS 6-7; Traveller
    4-7]
        Plastics, automobile, aircraft, tanks, radio, telephone, fission
        power, computers, guided missiles, satellites, nuclear weapons,
        automatic weapons
    IIIc: Cyberpunk, circa 2000 to 2100 AD ? [GURPS 8 (early); Traveller 8
    (early)]
        Fusion power, cyberspace, genetic engineering, nanotechnology,
        lasers
Group IV -- Interstellar technology
    IVa: STL interstellar, circa 2100 to 2200 AD ? [GURPS 8 (late);
    Traveller 8 (late)]
        Ramjet ships, terraforming, artificial intelligence
    IVb: FTL interstellar, circa 2200 to 3000 AD ? [GURPS 9-13; Traveller
    9-15]
        FTL travel, gravity control, mass conversion power
    IVc: Advanced interstellar, circa 3000 AD to ? [GURPS 14; Traveller
    16-21]
        Matter transmitter
Group V -- Kardashev type II civilisations
    V: Dysonian [GURPS 15; Traveller 22-27]
        Artificial worlds
Group VI -- Unknown technology
    VI: Unknown [GURPS 16+; Traveller 28+]
        Time travel


## INTELLIGENT LIFE

Obviously any system for designing intelligent aliens has to be based on at least as much personal preference and just plain wild guesswork as hard facts. Anyone who uses this system is urged to take a careful look at it first and make any changes you think will bring it more in line with your version of the universe.


### PHYSICAL DESCRIPTION

This is intended to be a generic system for generating intelligent or semi-intelligent species. Some minor modifications may be required to fit some details of the aliens' home world, if you've already generated it; most of these should be obvious enough that I don't need to spell them out (for example, if the planet has no life more advanced than invertebrates, you can exclude the vertebrates from the "metabolism and body structure" roll).

Find the normal environment of the species:

    D100   Environment
    -----  --------------
    1-80   Land-dwelling
    81-82  Burrowing
    83-94  Amphibious
    95-99  Aquatic
    100    Flying

Find the type of metabolism and body structure:

    D100    Metabolism and body structure
    ------  -----------------------------
    1-15    Cold-blooded invertebrate
    16-20   Warm-blooded invertebrate
    21-30   Cold-blooded vertebrate
    31-100  Warm-blooded vertebrate

Find the type of body covering:

    D100    Types of body covering
    ------  ----------------------
    1-75    One main type
    76-100  Two main types

    D100                                              Body covering
    Flying  Invertebrate  Cold-blooded  Warm-blooded
                          vertebrate    vertebrate
    ------  ------------  ------------  ------------  -------------
    1-10    1-25          1-10          1-20          Soft-skinned
    15-20   26-50         11-30         21-30         Thick-skinned
    21-40   51-60         31-35         31-90         Furred
    31-80   61            36            91            Feathered
    81-89   62-70         37-80         92-97         Scaled
    90      71-75         81-83         98            Spiny
    91-100  76-100        84-100        99-100        Hard-shelled

Use the first column for all flying creatures; otherwise, use the column appropriate to the creature's body type. If there are two types of body covering, re-roll the second if it comes out the same as the first.

Find the type of body symmetry and the number of limbs:

    D100                      Symmetry   Number of limbs
    Invertebrate  Vertebrate
    ------------  ----------  ---------  ---------------
    1-20          1-60        Bilateral  4
    21-40         61-90       ...        6
    41-60         91-95       ...        8
    61-80         96-97       ...        (D6+4)x2
    81-85         98          ...        (D100+10)x2
    86-95         99          Radial     5
    96-100        100         ...        D10+2

(If you're wondering why most of the creatures with radial symmetry have five limbs, it's not just Earth prejudice; there are good engineering reasons why five is the optimum number of limbs for a creature with radial symmetry. Having an even number of body segments is a bad idea, because it weakens the body by placing several continuous seams around it. A creature with three arms would probably be unable to survive if it lost one; five are much better for redundancy. There are some echinoderms on Earth with more than five limbs, but not many.)

For creatures with radial symmetry, all limbs are assumed to be dual purpose arm/legs. Flying creatures with radial symmetry are assumed to be lighter-than-air, balloon-like creatures.

For creatures with bilateral symmetry, roll once for each pair of limbs, except as noted below:

    D100    Type of limbs
    ------  --------------------------------------------------------------
    1-10    Wings if flying; fins if amphibious or aquatic; otherwise legs
    11-50   Fins if aquatic (not amphibious); otherwise legs
    51-70   Legs
    71-75   Dual-purpose arm/legs
    76-100  Arms

For flying creatures, assign one pair of limbs as wings without rolling (wings generated on the table are additional pairs). All intelligent creatures will have at least one pair of hands (either arms or arm/legs).  If you get a result that violates any of these checks, start again. If the creature has more than ten limbs, roll only for the first five pairs; the rest are all assumed to be legs.

Find the creature's diet:

    D100    Diet
    ------  -----------
    1-10    Herbivorous
    20-70   Omnivorous
    80-100  Carnivorous

Find the creature's method of reproduction:

    D100   Type of reproduction
    -----  --------------------
    1-5    Asexual
    6-25   Hermaphroditic
    25-99  Two sexes
    100    Three sexes

    D100                                      Method of reproduction
    Invertebrate  Cold-blooded  Warm-blooded
                  vertebrate    vertebrate
    ------------  ------------  ------------  ----------------------
    1-5           --            --            External budding
    6-80          1-70          1-30          Egg-laying
    81-100        71-100        31-100        Live-bearing

Find the average mass and size of the creature; roll 2D10 for land-dwelling or amphibious creatures, 2D10+3 for aquatic creatures, or 2D6 for flying or burrowing creatures:

    Result  Mass    Size
    ------  ------  ---------------
    2       2 kg    (2D6+5) x 4 cm
    3       5 kg    (2D6+5) x 6 cm
    4       10 kg   (2D6+5) x 8 cm
    5       15 kg   (2D6+5) x 9 cm
    6       20 kg   (2D6+5) x 10 cm
    7       30 kg   (2D6+5) x 11 cm
    8       40 kg   (2D6+5) x 12 cm
    9       50 kg   (2D6+5) x 13 cm
    10      60 kg   (2D6+5) x 14 cm
    11      75 kg   (2D6+5) x 15 cm
    12      100 kg  (2D6+5) x 16 cm
    13      150 kg  (2D6+5) x 18 cm
    14      200 kg  (2D6+5) x 21 cm
    15      300 kg  (2D6+5) x 24 cm
    16      500 kg  (2D6+5) x 28 cm
    17      1 t     (2D6+5) x 35 cm
    18      2 t     (2D6+5) x 45 cm
    19      5 t     (2D6+5) x 60 cm
    20      10 t    (2D6+5) x 75 cm
    21      20 t    (2D6+5) x 1 m
    22      50 t    (2D6+5) x 1.3 m
    23      100 t   (2D6+5) x 1.6 m

For flying creatures and snake-like creatures (any non-aquatic creatures without legs), multiply the size by 4. The size generated is the creature's greatest dimension -- height for humanoids, length for most horizontally oriented creatures, wingspan for flying creatures. Round the size to the nearest 10 centimetres (or 5 centimetres if it's less than one metre).

### SPECIAL FEATURES

This section covers the sort of features that many role-playing games treat as advantages and disadvantages -- natural weapons, unusually fast or slow speed, non-human senses, and so forth. Some features relevant to your game mechanics will have already been generated, such as the ability to fly or swim, extra hands, or whatever degree of natural armour is implied by the creature's body covering.

Attributes such as strength, dexterity, intelligence and so on are too game-specific to be covered here. You'll have to wing it.

Roll D6-3 to determine how many special features the species has. Then roll D100 on the following table the appropriate number of times; re-roll any repeated results. Some of the entries are double (e.g. "acute vision/poor vision"); the two are mutually exclusive, and there is a fifty-fifty chance of one or the other. The "acute" or "poor" senses are relative to human senses (which is why there's no "poor smell" feature -- the human sense of smell is pretty poor to start with).

I haven't included precise definitions of the effects of each of these special features; any details beyond what is implied by the names would have to be worked out to fit your particular game mechanics.

    D100                            Special abilities
    Herbivore  Omnivore  Carnivore
    ---------  --------  ---------  ------------------------------------
    1-18       1-17      1-16       Acute hearing/poor hearing
    19-30      18-28     17-26      Acute smell
    31-48      29-45     27-42      Acute vision/poor vision
    49-60      46-56     43-52      Ambidextrous
    61-62      57-58     53-54      Chameleon skin
    63-68      59-64     55-59      Cold sensitivity/cold tolerance [*1]
    69-74      65-70     60-64      Colour blind
    75-80      71-76     65-69      Heat sensitivity/heat tolerance [*1]
    81-86      77-82     70-74      Infrared vision
    87-91      83-88     75-84      Night vision
    92         89-91     85-89      Poison
    93         92        90         Radiation tolerance
    94         93        91         Radio communication
    95         94        92         Radio sense
    96         95        93         Ranged weapon
    97         96        94         Regeneration
    98         97-98     95-97      Sonar [*2]
    99         99        98         Suckers (wall climbing)
    100        100       99         Vacuum tolerance
    --         --        100        Web spinning

    [*1: If you're creating an intelligent species for an already-generated
    planet, the planet's surface temperature will affect the natives'
    heat/cold tolerance. If the temperature -5 degrees or less, the natives
    automatically have cold tolerance, and have a 50%25 chance of heat
    sensitivity; ignore and re-roll any of the [*1] results. If the
    temperature is 35 degrees or higher, the natives automatically have
    heat tolerance, and have a 50%25 chance of cold sensitivity; ignore and
    re-roll any of the [*1] results. If the temperature is 0 to 30 degrees,
    generate as above.]

    [*2: Sonar implies acute hearing; add acute hearing to your list of
    features (don't count it towards the total), and ignore any other rolls
    of acute/poor hearing.]

Two other special features are determined separately: natural weapons and speed.

The chance that the aliens will have natural weapons (claws, fangs, horns, or whatever) is 20%25 for herbivores, 40%25 for omnivores, and 80%25 for carnivores. This refers only to close-combat weapons; ranged weapons are generated separately from the table above.

Roll 2D6 on the following table to find the aliens' running (or swimming or flying) speed, relative to human speed. Add 1 for carnivores. For land or water creatures, subtract 2 if their average body mass is less than 10 kilograms. For flying creatures, don't adjust for mass, and double the speed (the final multiplier, not the die roll).

    Result  Speed
    ------  -----
    0-3     x1/2
    4-9     x1
    10-11   x2
    12      x3
    13      x4

### PSYCHOLOGICAL PROFILE

The psychological profile of an intelligent species is described by a set of six numbers: social, cooperation, aggression, exploration, technology, and art. Each runs from 0 to 100.

Social: Indicates the degree of gregariousness and social organisation in their civilisation. A social rating of zero would indicate a totally solitary species with no social interaction at all; a social rating of 100 would indicate a hive-mind species with no concept of individual identity.  Some social contact is assumed to be required for the evolution of language and intelligence, so a social rating less than 5 is not allowed in this system.

Cooperation: Indicates how willing they are to cooperate with other intelligent species. A cooperation rating of zero would indicate a totally xenophobic species that refuses to even recognise the existence of any other intelligent life; a cooperation rating of 100 would indicate a race with no sense of species identity at all, making no distinction between their own conspecifics and aliens.

Aggression: Indicates how warlike they are, both among themselves and against other species. An aggression rating of zero would indicate a completely pacifist species that never fought anyone for any reason; an aggression rating of 100 would indicate a completely warlike species with no interest in any other activity. For obvious reasons there will be a negative correlation between the cooperation and aggression ratings (but not completely -- for example, a species that enjoyed fighting and frequently hired themselves out as mercenaries to anyone who needed soldiers might have a high rating in both areas, while a peaceful but isolationist species, such as Larry Niven's Puppeteers, would have a low rating in both).

Exploration: Indicates their curiosity and interest in research and exploring the universe. An exploration rating of zero would indicate a species with no curiosity at all (since this seems incompatible with intelligence, a rating of less than 5 is not allowed); an exploration rating of 100 would indicate a species completely obsessed with exploration or science.

Technology: Indicates their technological aptitude. A technology rating of zero would indicate a species with no technology of any kind; a technology rating of 100 would indicate a species obsessed with technology to the exclusion of anything else. There is a strong positive correlation between the exploration and technology ratings.

Art: Indicates what part artistic activities play in their society. An art rating of zero would indicate a completely practical and utilitarian species, with no aesthetic sense at all (to humans they would seem cold and robotic); an art rating of 100 would indicate that aesthetic considerations completely dominated practical ones (this would not be a survival trait, which is why an art rating above 95 is not allowed). There is a negative correlation between the technology and art ratings.

    Profile      Basic                            Modifiers      Allowed
    element      die roll                                        range
    -----------  -------------------------------  -------------  -------
    Social       (2D6x10)+D10-25                  Herbivore +10  5-100
                                                  Omnivore  0
                                                  Carnivore -10
    Cooperation  (2D6x10)+D10-25                  Herbivore 0    0-100
                                                  Omnivore  +5
                                                  Carnivore -5
    Aggression   (2D6x10)+D10-(Cooperation/5)-15  Herbivore -10  0-100
                                                  Omnivore  0
                                                  Carnivore +10
    Exploration  (2D6x10)+D10-25                  Herbivore -10  5-100
                                                  Omnivore  +5
                                                  Carnivore +5
    Technology   (D6x10)+D10+(Exploration/2)-15   --             0-100
    Art          (2D6x10)+D10-(Technology/5)-15   --             0-95

If the result is outside the allowed range, roll again.

### TECHNOLOGY

To find a race's typical technology level, roll 2D10, add one-fifth of their technological aptitude (from the psychological profile), and refer to the following table:

    TL roll  Tech level
    -------  --------------------------
    0-6      No technology
    7-13     I: Stone age
    14       IIa: Bronze age
    15       IIb: Classical/mediaeval
    16       IIc: Renaissance
    17       IIIa: Steam age
    18       IIIb: Twentieth century
    19       IIIc: Cyberpunk
    20       IVa: STL interstellar
    21-25    IVb: FTL interstellar
    26-34    IVc: Advanced interstellar
    35-38    V: Dysonian
    39+      VI: Unknown

### 7.5. EXAMPLES

Descriptions of the human race and two alien races:

Human -- Land-dwelling, warm-blooded vertebrate, soft-skinned, bilateral

symmetry, 4 limbs (2 arms, 2 legs), omnivorous, two sexes, live-bearing, mass 75 kg, size 1.8 m, speed x1; Soc 65, Coop 55, Aggr 65, Expl 75, Tech 65, Art 45; tech level IIIb (twentieth century)

Alien 1 -- Land-dwelling, warm-blooded vertebrate, furred, bilateral

symmetry, 6 limbs (2 arms, 4 legs), carnivorous, hermaphroditic, live-bearing, mass 20 kg, size 1.4 m, speed x2; natural weapons; Soc 63, Coop 54, Aggr 17, Expl 31, Tech 52, Art 72; tech level IVb (FTL interstellar)

Alien 2 -- Amphibious, cold-blooded vertebrate, scaled, bilateral symmetry,

4 limbs (2 arm/legs, 2 legs), herbivorous, two sexes, egg-laying, mass 200 kg, size 2.9 m, speed x1; acute hearing, heat sensitivity; Soc 52, Coop 73, Aggr 67, Expl 51, Tech 75, Art 50; tech level IVc (advanced interstellar)

---

Ross Smith ........................................ Wellington, New Zealand
Home: %3calien@netlink.co.nz> ................. Work: %3cross.smith@nz.eds.com>
          "Those who do not remember the past are condemned to
          watch the mini-series."             -- Diana Wichtel
