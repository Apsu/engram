# Arno's Engram key layout

The [Engram layout](https://github.com/binarybottle/engram-layout) is a keyboard layout optimized for comfortable touch typing in English created by [Arno Klein](https://binarybottle.com), with open source code to create other optimized key layouts.

               Y  O  U  K        W  M  D  B
               I  H  E  A        R  T  S  N
               V  Z  X  C        L  G  F  P

The Shift key accesses characters (top) that look similar to the numbers:

               !  =  ?  +  $  @  ^  &  %  *
               1  2  3  4  5  6  7  8  9  0

and accesses related but less common punctuation (top):

            `    \    ;    :    {    }    |    _
            '    "    ,    .    (    )    /    -

Swapping the Backspace and Caps lock keys completes the layout:

    ~          !  =  ?  +  $  @  ^  &  %  *  <  >
    #          1  2  3  4  5  6  7  8  9  0  [  ]     Caps

    Tab        Y  O  U  K  '  "  W  M  D  B  Q  -     /
    Back       I  H  E  A  ,  .  R  T  S  N  J        Enter
    Shift      V  Z  X  C  (  )  L  G  F  P           Shift

    Ctrl   Fn  Cmd  Alt    Space     Alt  Ctrl       Arrows    
    

## Rationale <a name="rationale">

**Why?** <br>
In the future, I hope to include an engaging rationale for why I took on this challenge.
Suffice to say that I have battled repetitive strain injury since I worked
on an old DEC workstation at the MIT Media Lab while composing my thesis back in the mid-90s.
Ever since then I have used different key layouts (Dvorak, Colemak, my own, etc.),
and have primarily used Colemak for almost 10 years.  I find that they all place too much stress on tendons, with lateral extension of the index and little fingers,
and on uniform distribution of finger use, which has damaged my little fingers.
I have also experimented with a wide variety of human interface technologies
(voice dictation, one-handed keyboard, keyless keyboard, foot mouse, and ergonomic keyboards like the Kinesis Advantage. I recently got an Ergodox that I am looking forward to trying out with the Engram layout.

**"Engram"?** <br>
The name is a pun, referring both to "n-gram", letter permutations used to compute this layout, and "engram", or memory trace, the postulated change in neural tissue to account for the persistence of memory.

## Comparison with other key layouts <a name="comparison">

Despite the fact that the Engram layout was designed to reduce strain and discomfort, not to reduce finger travel from the home row, it scores higher than all other key layouts (Colemak, Dvorak, QWERTY, etc.) I've tested using the online Keyboard Layout Analyzer, for all of the examples of prose and tweet data I've tried, including the data sets below:

- [See the complete analysis](http://patorjk.com/keyboard-layout-analyzer/#/load/x0WPtw3x)
of __Alice in Wonderland__ provided by the Keyboard Layout Analyzer 

- All __20,000 tweets__ from [Gender Classifier Data](https://www.kaggle.com/crowdflower/twitter-user-gender-classification) <br>
Added: November 15, 2015 by CrowdFlower

- The first __100,000 tweets__ from: [Sentiment140 dataset](https://data.world/data-society/twitter-user-data) training data <br>
Go, A., Bhayani, R. and Huang, L., 2009. <br>
Twitter sentiment classification using distant supervision. <br>
CS224N Project Report, Stanford, 1(2009), p.12.

According to the [Keyboard Layout Analyzer](http://patorjk.com/keyboard-layout-analyzer/):

"The optimal layout score is based on a weighted calculation that factors in the distance your fingers moved (33%), how often you use particular fingers (33%), and how often you switch fingers and hands while typing (34%)."
    
From the [Internet Letter Layout DB](https://www.keyboard-design.com/internet-letter-layout-db.html) for ANSI/ISO layouts:

    - [Halmak](https://www.keyboard-design.com/letterlayout.html?layout=halmak-2-2.en.ansi)
    - [Workman](https://www.keyboard-design.com/letterlayout.html?layout=workman.en.ansi)
    - [Norman](https://www.keyboard-design.com/letterlayout.html?layout=norman.en.ansi)
    - [Colemak](https://www.keyboard-design.com/letterlayout.html?layout=colemak.en.ansi)
    - [Dvorak](https://www.keyboard-design.com/letterlayout.html?layout=dvorak.en.ansi)
    - [Qwerty](https://www.keyboard-design.com/letterlayout.html?layout=qwerty.en.ansi)
    
## Factors used to compute the layout <a name="factors">
  - **N-gram letter frequencies** <br>
    
    [Peter Norvig's analysis](http://www.norvig.com/mayzner.html) of data from Google's book scanning project
  - **Flow factors** (transitions between ordered key pairs) <br>
    These factors are influenced by Dvorak's 11 criteria (1936).
  - **Finger strengths** (peak keyboard reaction forces) <br>
      "Keyboard Reaction Force and Finger Flexor Electromyograms during Computer Keyboard Work", BJ Martin, TJ Armstrong, JA Foulke, S Natarajan, Human Factors,1996,38(4),654-664.
  - **Speed** (unordered interkey stroke times) <br>
      "Estimation of digraph costs for keyboard layout optimization", A Iseri, Ma Eksioglu, International Journal of Industrial Ergonomics, 48, 127-138, 2015. <br>
      _NOTE: Speed data were only used for exploration of early key layouts._
      
## Guiding criteria   <a name="criteria">

1.  Assign 24 letters to columns of keys that don't require lateral finger movement.
2.  Assign common punctuation to keys in the middle columns of the keyboard.
3.  Assign easier-to-remember characters to the shift-number keys.
4.  Group letters for common command shortcuts close together.
5.  Arrange letters so that more frequent bigrams are faster and easier to type.
6.  Balance finger loads according to their relative strength.
7.  Promote alternating between hands over uncomfortable transitions with the same hand.
8.  Promote little-to-index-finger roll-ins over index-to-little-finger roll_outs.
9.  Avoid stretching shorter fingers up and longer fingers down.
10. Avoid using the same finger.
11. Avoid the upper and lower rows.
12. Avoid skipping over the home row.

## Summary of steps and results  <a name="summary">

- Step 1: Define the shape of the key layout to minimize lateral finger movements
- Step 2: Assign command shortcut letters to the bottom left row
- Step 3: Arrange the most frequent letters based on comfort and bigram frequencies
- Step 4: Optimize assignment of the remaining letters
- Step 5: Arrange non-letter characters in easy-to-remember places

### 1: Define the shape of the key layout to minimize lateral finger movements

We will assign 24 letters to 8 columns of keys separated by two middle columns reserved for punctuation. These 8 columns require no lateral finger movements when touch typing, since there is one column per finger. The most comfortable keys include the left and right home rows (keys 5-8 and 17-20), the top-center keys (2,3 and 14,15) that allow the longer middle and ring fingers to uncurl upwards, as well as the bottom corner keys (9,12 and 21,24) that allow the shorter fingers to curl downwards. We will reserve the bottom left row (keys 9-12) for common command shortcut letters (Z,X,C,V), and will reserve the two hardest-to-reach keys lying outside the 24-key columns in the upper right to the two least frequent remaining letters, Q and J:

        Left:            Right:
     1  2  3  4       13 14 15 16  Q
     5  6  7  8       17 18 19 20  J
    [9 10 11 12]      21 22 23 24

### 2: Assign command shortcut letters to the bottom left row

We begin by assigning the common command letters V,Z,X,C to the bottom left row. We place V and Z to the left of X and C, because V and Z are often repeated (to paste multiple times or to undo multiple mistakes) whereas C and X are not (the copy and cut buffers are overwritten), and should lie closer to the Ctrl/Cmd key for ease of access with one hand. V and C are assigned to the most comfortable of the four keys (as noted above) because they are more frequent letters in English than Z and X.

     -  -  -  -        -  -  -  -
     -  -  -  -        -  -  -  -
     V  Z  X  C        -  -  -  -

### 3: Arrange the most frequent letters based on comfort and bigram frequencies  <a name="step3">

In prior experiments using the methods below, all vowels automatically clustered together, with the most frequent letters assigned to the strongest fingers (in order: middle, index, ring, little), and the letter Y consistently landed in the top left key for the highest-scoring layouts. Below, we will arrange vowels to the left side and the most frequent consonants to the right side to encourage balance and alternation across hands.
    
#### Vowels
    
**E**, T, **A, O, I**, N, S, R, H, L, D, [C], **U**, M, F, P, G, W, **Y**, B, [V], K, [X], J, Q, [Z]

We will assign the four most frequent vowels (E,A,O,I) to the most comfortable keys in the left home and upper rows (keys 5-8 and 2-3), with the letter E, the most frequent in the English language, assigned to either of the strongest keys (7 and 8, the middle and index fingers on the left home row). The letter U may also take the less comfortable key 4. We will arrange the vowels such that any top-frequency bigram (more than 1 billion instances in Peter Norvig's analysis of Google data) reads from left to right (ex: TH, not HT) for ease of typing (roll-in from little to index finger vs. roll-out from index to little finger). These constraints lead to comfortable and efficient layouts:
    
    (1)  Y  O  U  -
         I  -  E  A    

    (2)  Y  -  U  - 
         I  O  E  A      

    (3)  Y  -  -  U 
         I  O  E  A      

    (4)  Y  -  O  U   
         I  -  E  A    

    (5)  Y  -  O  U   
         -  I  E  A    

    (6)  Y  I  O  U    
         -  -  E  A     

#### Consonants

Next, to populate the home row on the right side, we examine all possible sequences of four letters from the seven most frequent consonants (T,N,S,R,H,L,D):

E, **T**, A, O, I, **N, S, R, H, L, D**, [C], U, M, F, P, G, W, Y, B, [V], K, [X], J, Q, [Z]

These seven consonants are included in the highest frequency bigrams listed below, with more than 1 billion instances in Peter Norvig's analysis:

**TH, ND, ST, NT, NS, TR, RS**, (RT), SH, LD, RD, LS, DS, LT, (TL), RL, HR, NL, (SL)

To maximize the number of bigrams we can comfortably type, we select 4-consonant sequences that consist of three consecutive highest frequency bigrams, such as NSTR = NS + ST + TR. We also restrict T and R to the strongest (middle or index) fingers, because T is the most frequent consonant, and the letter R needs to be preceded by other consonants to comfortably type frequent bigrams (TR,DR,HR,PR,FR,BR,GR, etc.) by rolling in from little-to-index finger.

    N  S  T  R
    N  L  T  R
    D  S  T  R    
    N  S  T  H
    N  L  T  H    
    L  S  T  H    
    D  S  T  H    
    N  L  S  T      
    N  D  S  T    
    L  D  S  T    
    
When reordered from right-to-left for ease of typing with the right hand, we have 10 consonant sequences:
    
    (0) RTSN
    (1) RTLN
    (2) RTSD
    (3) HTSN
    (4) HTLN
    (5) HTSL
    (6) HTSD
    (7) TSLN
    (8) TSDN
    (9) TSDL
    
The resulting 6 arrangements of five vowels on the left and 10 arrangements of four consonants on the right gives us 60 possible layouts, each with 10 unassigned keys:

          Left hand         Right hand
    10  YOU- I-EA VZXC    ---- RTSN ----
    11  YOU- I-EA VZXC    ---- RTLN ----
    12  YOU- I-EA VZXC    ---- RTSD ----
    13  YOU- I-EA VZXC    ---- HTSN ----
    14  YOU- I-EA VZXC    ---- HTLN ----
    15  YOU- I-EA VZXC    ---- HTSL ----
    16  YOU- I-EA VZXC    ---- HTSD ----
    17  YOU- I-EA VZXC    ---- TSLN ----
    18  YOU- I-EA VZXC    ---- TSDN ----
    19  YOU- I-EA VZXC    ---- TSDL ----

    20  Y-U- IOEA VZXC    ---- RTSN ----
    21  Y-U- IOEA VZXC    ---- RTLN ----
    22  Y-U- IOEA VZXC    ---- RTSD ----
    23  Y-U- IOEA VZXC    ---- HTSN ----
    24  Y-U- IOEA VZXC    ---- HTLN ----
    25  Y-U- IOEA VZXC    ---- HTSL ----
    26  Y-U- IOEA VZXC    ---- HTSD ----
    27  Y-U- IOEA VZXC    ---- TSLN ----
    28  Y-U- IOEA VZXC    ---- TSDN ----
    29  Y-U- IOEA VZXC    ---- TSDL ----

    30  Y--U IOEA VZXC    ---- RTSN ----
    31  Y--U IOEA VZXC    ---- RTLN ----
    32  Y--U IOEA VZXC    ---- RTSD ----
    33  Y--U IOEA VZXC    ---- HTSN ----
    34  Y--U IOEA VZXC    ---- HTLN ----
    35  Y--U IOEA VZXC    ---- HTSL ----
    36  Y--U IOEA VZXC    ---- HTSD ----
    37  Y--U IOEA VZXC    ---- TSLN ----
    38  Y--U IOEA VZXC    ---- TSDN ----
    39  Y--U IOEA VZXC    ---- TSDL ----
    
    40  Y-OU I-EA VZXC    ---- RTSN ----
    41  Y-OU I-EA VZXC    ---- RTLN ----
    42  Y-OU I-EA VZXC    ---- RTSD ----
    43  Y-OU I-EA VZXC    ---- HTSN ----
    44  Y-OU I-EA VZXC    ---- HTLN ----
    45  Y-OU I-EA VZXC    ---- HTSL ----
    46  Y-OU I-EA VZXC    ---- HTSD ----
    47  Y-OU I-EA VZXC    ---- TSLN ----
    48  Y-OU I-EA VZXC    ---- TSDN ----
    49  Y-OU I-EA VZXC    ---- TSDL ----

    50  Y-OU -IEA VZXC    ---- RTSN ----
    51  Y-OU -IEA VZXC    ---- RTLN ----
    52  Y-OU -IEA VZXC    ---- RTSD ----
    53  Y-OU -IEA VZXC    ---- HTSN ----
    54  Y-OU -IEA VZXC    ---- HTLN ----
    55  Y-OU -IEA VZXC    ---- HTSL ----
    56  Y-OU -IEA VZXC    ---- HTSD ----
    57  Y-OU -IEA VZXC    ---- TSLN ----
    58  Y-OU -IEA VZXC    ---- TSDN ----
    59  Y-OU -IEA VZXC    ---- TSDL ----
    
    60  YIOU --EA VZXC    ---- RTSN ----
    61  YIOU --EA VZXC    ---- RTLN ----
    62  YIOU --EA VZXC    ---- RTSD ----
    63  YIOU --EA VZXC    ---- HTSN ----
    64  YIOU --EA VZXC    ---- HTLN ----
    65  YIOU --EA VZXC    ---- HTSL ----
    66  YIOU --EA VZXC    ---- HTSD ----
    67  YIOU --EA VZXC    ---- TSLN ----
    68  YIOU --EA VZXC    ---- TSDN ----
    69  YIOU --EA VZXC    ---- TSDL ----
    
### 4: Optimize assignment of the remaining letters

We will assign missing letters to the above layouts by scoring every possible arrangement of these 10 letters and selecting the top-scored arrangement. Since there are 3,628,800 (10 factorial) possible permutations for 10 letters, and we have 60 possible layouts each with 10 missing letters, we need to score and evaluate 217,728,000 permutations.  
    
To score each arrangement of letters, we construct a frequency matrix of each ordered pair of letters (bigram), and multiply this frequency matrix by our speed-strength-flow matrix to compute a score. 
    
The 10 missing letters in each layout are among those in bold below:

E, T, A, O, I, N, **S, R, H, L, D**, C, U, **M, F, P, G, W**, Y, **B**, V, **K**, X, J, Q, Z    

#### **Scoring details**
    
The optimization algorithm finds every permutation of a given set of letters, maps these letter permutations to a set of keys, and ranks these letter-key mappings according to a score reflecting ease of typing key pairs and frequency of letter pairs (bigrams). The score is the average of the scores for all possible bigrams in this arrangement. The score for each bigram is a product of the frequency of occurrence of that bigram and the factors Flow, Strength, and Speed: 

**Flow**: measure of ease of a finger transition from the first in a pair of letters to the second

Flow factors to _penalize_ difficult key transitions include:
    
- roll out from index to little finger
- index or little finger on top row
- middle or ring finger on bottom row
- index above middle, or little above ring 
- index above ring, or little above middle
- ring above middle
- use same finger twice for a non-repeating letter
- at least one key not on home row
- one key on top row, the other on bottom row

**Strength**: measure of the average strength of the finger(s) used to type the two letters

Finger strengths are based on peak keyboard reaction forces (in newtons) from "Keyboard Reaction Force and Finger Flexor Electromyograms during Computer Keyboard Work", BJ Martin, TJ Armstrong, JA Foulke, S Natarajan, Human Factors,1996, 38(4), 654-664.

**Speed**: normalized interkey stroke times

These are left-right averaged versions derived from the study data below, to compensate for right-handedness of participants in the study (we used this data for early experimentation):

"Estimation of digraph costs for keyboard layout optimization", 
A Iseri, Ma Eksioglu, International Journal of Industrial Ergonomics, 48, 127-138, 2015. 

### 5. Arrange non-letter characters in easy-to-remember places

Now that we have all 26 letters accounted for, we turn our attention to non-letter characters, taking into account frequency of punctuation and ease of recall.
    
**Frequency of punctuation** 

These sources helped guide our arrangement:
    
  - "Punctuation Input on Touchscreen Keyboards: Analyzing Frequency of Use and Costs" <br>
    S Malik, L Findlater - College Park: The Human-Computer Interaction Lab. 2013 <br>
    https://www.cs.umd.edu/sites/default/files/scholarly_papers/Malik.pdf

  - "Frequencies for English Punctuation Marks" by Vivian Cook <br>
    http://www.viviancook.uk/Punctuation/PunctFigs.htm

  - "Computer Languages Character Frequency" <br>
    Xah Lee. Date: 2013-05-23. Last updated: 2020-06-29. <br>
    http://xahlee.info/comp/computer_language_char_distribution.html

#### Add punctuation keys and number keys

Shift to access similar-looking characters above the numbers, and swap the Backspace and Caps lock keys:


    ~          !  =  ?  +  $  @  ^  &  %  *  <  >
    #          1  2  3  4  5  6  7  8  9  0  [  ]     Caps

    Tab        Y  O  U  K  '  "  W  M  D  B  Q  -     /
    Back       I  H  E  A  ,  .  R  T  S  N  J        Enter
    Shift      V  Z  X  C  (  )  L  G  F  P           Shift

    Ctrl   Fn  Cmd  Alt    Space     Alt  Ctrl       Arrows


Shift accesses similar-looking characters above the numbers:

     !  =  ?  +  $  @  ^  &  %  *  [  ]
     1  2  3  4  5  6  7  8  9  0  <  >

Shift accesses less common, but similar-meaning punctuation:

     `    \    ;    :    {    }    |    _
     '    "    ,    .    (    )    /    -
             
**Rationale for shift-characters**

**#** &nbsp;&nbsp; The pound/hash represents numbers, and sits to the left of the number keys. <br>
**~** &nbsp;&nbsp; The tilde has several meanings, including "approximately equal to" <br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (here "similar-looking" to the numbers), and is in the standard location.

**'** &nbsp;&nbsp; Single quotation marks are used to quote text for 'emphasis', or to quote text within a quote. <br>
**`** &nbsp;&nbsp; One use of the backquote is to quote computer code. It is used in an analogous manner as a single quote <br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; in a quote, to quote code within code for command substitution (to replace a command with output).

**"** &nbsp;&nbsp; "Double quotation marks are used to quote direct speech?" <br>
**\** &nbsp;&nbsp; The backslash is an escape character used to quote special characters in regular expressions.

**,** &nbsp;&nbsp; The comma is used to separate text, for example in lists, or to provide a pause. <br>
**;** &nbsp;&nbsp; The semicolon provides a stronger separation or pause; it can be used in place <br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; of the comma to separate items in a list, especially if those items contain commas. <br>
   
**.** &nbsp;&nbsp; The period ends a sentence. <br>
**:** &nbsp;&nbsp; The colon similarly ends a statement but precedes something following: explanation, quotation, list, etc.

**|** &nbsp;&nbsp; The pipe connects commands in computer code. <br>
**/** &nbsp;&nbsp; The slash connects conjunctions/disjunctions/alternatives, or locations such as file paths or urls.

**-** &nbsp;&nbsp; The dash connects side-by-side words, or can surround a phrase for emphasis. <br>
**_** &nbsp;&nbsp; The underscore connects strings within variable or file names, or can _underline a phrase_ for emphasis.
