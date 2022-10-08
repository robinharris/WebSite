---
layout: post
title: EFHW Matching
date: 2022-10-06 08:30
Categories: EFHW
---
I have an End Fed Half Wave (EFHW) aerial at home.  It is 39m long in an inverted vee shape with the apex at 12m.  The first matching unit used an FT114-43 toroidal core wound 3:21 to provide a 49:1 impedance transformation.  A 100pF capacitor was included to improve the efficiency on the higher bands.

In comparisons with a portable EFHW at lower height in the garden the home aerial performed worse with received signals being 1 or 2 S points down.

After eliminating possible causes such as the feeder and poor connections it looked very much like the problem was in the matching unit.  A visual check confirmed that there was nothing obviously wrong - it was clean and dry with sound connections.

After following the work of Colin (MM0OPX) on transformer efficiency I decided to try a different core - the 2643625002 came out very well in his tests for QRP power levels.  I wound onto one othe these cores an autotransformer with 3:21 ratio.  Bench tests using a pair of transformers back to back showed very good efficiency from 3.5MHz to 14Mhz without a compensation capacitor but above this it fell away.  The optimum value for compensation turned out to be 150pF

{:style="text-align:center;"}
![Losses](/WebSite/images/transformer_test1.jpg){:width="40% height="25%"}
![Losses](/WebSite/images/transformer_test2.jpg){:width="40% height="25%"}
