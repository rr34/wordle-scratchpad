# Wordle Scratchpad by Nate
## The User Interface
The UI is very unusual. I was experimenting with keyboard-only operation and wanted to make all user inputs go through the 'clipboard.' Therefore, the 'flow' of using the program is as follows:
`<t>` type your guess
`<Enter>` puts the guess on the clipboard
`<g>` to transfer from the clipboard to guess in the program
`<t>` type your hint
`<Enter>` places hint on the clipboard
`<h>` transfer the hint from clipboard to hint in the program
At this point, you should see an output showing the number of remaining possible solutions based on the guess and hint you entered.
`<c>` and you will see a list of the top-10 next guesses based on the scoring described in the below log file from an actual run of the program.
Use the recommended guesses to make another guess in Wordle then repeat the steps above for your second guess and so on.
`<s>` is used to transfer from the clipboard to practice solution.
`<a>` is used to transfer from the clipboard to practice guess and the program will show the Wordle hint based on the solution-guess combination.

## Log File
If you play Wordle, you will immediately recognize the value of this output:

Parsed Webster's Unabridged Dictionary into list in 1.4654310879999954 seconds.
RAISE: guess #1
BBBBG: hint #1
From 6246 words to 254 words in 0.009 seconds.
Counted word list letters, sorted by frequency in 0.038904385000009256 seconds.
Letters ranked by likelihood of single appearance in word list:
'E' frequency, positional: [0.087, 0.236, 0.106, 0.039, 1.0], by letter: 0.294, by word appearance: 1.0
'O' frequency, positional: [0.028, 0.315, 0.142, 0.008, 0.0], by letter: 0.098, by word appearance: 0.469
'L' frequency, positional: [0.075, 0.122, 0.087, 0.193, 0.0], by letter: 0.095, by word appearance: 0.457
'U' frequency, positional: [0.016, 0.11, 0.11, 0.047, 0.0], by letter: 0.057, by word appearance: 0.268
'N' frequency, positional: [0.039, 0.028, 0.126, 0.067, 0.0], by letter: 0.052, by word appearance: 0.228
'D' frequency, positional: [0.059, 0.008, 0.091, 0.075, 0.0], by letter: 0.046, by word appearance: 0.22
'G' frequency, positional: [0.051, 0.0, 0.051, 0.122, 0.0], by letter: 0.045, by word appearance: 0.209
'T' frequency, positional: [0.063, 0.012, 0.063, 0.094, 0.0], by letter: 0.046, by word appearance: 0.193
'C' frequency, positional: [0.083, 0.004, 0.043, 0.051, 0.0], by letter: 0.036, by word appearance: 0.173
'H' frequency, positional: [0.051, 0.067, 0.004, 0.055, 0.0], by letter: 0.035, by word appearance: 0.173
'M' frequency, positional: [0.075, 0.016, 0.016, 0.059, 0.0], by letter: 0.033, by word appearance: 0.157
'B' frequency, positional: [0.091, 0.004, 0.016, 0.024, 0.0], by letter: 0.027, by word appearance: 0.134
'Y' frequency, positional: [0.008, 0.047, 0.055, 0.012, 0.0], by letter: 0.024, by word appearance: 0.122
'P' frequency, positional: [0.063, 0.004, 0.02, 0.028, 0.0], by letter: 0.023, by word appearance: 0.114
'V' frequency, positional: [0.024, 0.012, 0.008, 0.059, 0.0], by letter: 0.02, by word appearance: 0.102
'F' frequency, positional: [0.091, 0.0, 0.004, 0.004, 0.0], by letter: 0.02, by word appearance: 0.094
'W' frequency, positional: [0.039, 0.0, 0.031, 0.008, 0.0], by letter: 0.016, by word appearance: 0.075
'K' frequency, positional: [0.028, 0.0, 0.012, 0.024, 0.0], by letter: 0.013, by word appearance: 0.063
'Z' frequency, positional: [0.008, 0.004, 0.004, 0.028, 0.0], by letter: 0.009, by word appearance: 0.043
'Q' frequency, positional: [0.016, 0.0, 0.012, 0.0, 0.0], by letter: 0.006, by word appearance: 0.028
'J' frequency, positional: [0.008, 0.0, 0.0, 0.004, 0.0], by letter: 0.002, by word appearance: 0.012
'X' frequency, positional: [0.0, 0.012, 0.0, 0.0, 0.0], by letter: 0.002, by word appearance: 0.012
'A' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'I' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'R' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'S' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0

Words ranked by sum of each letter positional frequency + word appearance frequency (each unique letter single count, so repeat letters don't add) in 0.025330791000001796 seconds.
Words ranked:
1. ('NOULE', [0.039, 0.315, 0.11, 0.193, 1.0], 4.079)
2. ('MOULE', [0.075, 0.315, 0.11, 0.193, 1.0], 4.044)
3. ('CODLE', [0.083, 0.315, 0.091, 0.193, 1.0], 4.001)
4. ('LONGE', [0.075, 0.315, 0.126, 0.122, 1.0], 4.0009999999999994)
5. ('FOULE', [0.091, 0.315, 0.11, 0.193, 1.0], 3.9969999999999994)
6. ('BODLE', [0.091, 0.315, 0.091, 0.193, 1.0], 3.97)
7. ('LODGE', [0.075, 0.315, 0.091, 0.122, 1.0], 3.958)
8. ('BOGLE', [0.091, 0.315, 0.051, 0.193, 1.0], 3.919)
9. ('NOLDE', [0.039, 0.315, 0.087, 0.075, 1.0], 3.8900000000000006)
10. ('YODLE', [0.008, 0.315, 0.091, 0.193, 1.0], 3.875)
11. ('NOBLE', [0.039, 0.315, 0.016, 0.193, 1.0], 3.851)
12. ('MOYLE', [0.075, 0.315, 0.055, 0.193, 1.0], 3.843)
13. ('COBLE', [0.083, 0.315, 0.016, 0.193, 1.0], 3.84)
14. ('JOULE', [0.008, 0.315, 0.11, 0.193, 1.0], 3.8319999999999994)
15. ('VOGLE', [0.024, 0.315, 0.051, 0.193, 1.0], 3.82)
16. ('DOWLE', [0.059, 0.315, 0.031, 0.193, 1.0], 3.8190000000000004)
17. ('MOBLE', [0.075, 0.315, 0.016, 0.193, 1.0], 3.816)
18. ('VOLGE', [0.024, 0.315, 0.087, 0.122, 1.0], 3.7849999999999997)
19. ('DHOLE', [0.059, 0.067, 0.142, 0.193, 1.0], 3.7800000000000002)
20. ('GHOLE', [0.051, 0.067, 0.142, 0.193, 1.0], 3.761)
21. ('LOCHE', [0.075, 0.315, 0.043, 0.055, 1.0], 3.7600000000000002)
22. ('THOLE', [0.063, 0.067, 0.142, 0.193, 1.0], 3.757)
23. ('NOZLE', [0.039, 0.315, 0.004, 0.193, 1.0], 3.748)
24. ('GLODE', [0.051, 0.122, 0.142, 0.075, 1.0], 3.745)
25. ('WOLDE', [0.039, 0.315, 0.087, 0.075, 1.0], 3.7370000000000005)
26. ('CLOTE', [0.083, 0.122, 0.142, 0.094, 1.0], 3.7329999999999997)
27. ('TONGE', [0.063, 0.315, 0.126, 0.122, 1.0], 3.725)
28. ('CONGE', [0.083, 0.315, 0.126, 0.122, 1.0], 3.725)
29. ('BOUGE', [0.091, 0.315, 0.11, 0.122, 1.0], 3.718)
30. ('DOOLE', [0.059, 0.315, 0.142, 0.193, 1.0], 3.713)
31. ('BLOTE', [0.091, 0.122, 0.142, 0.094, 1.0], 3.7019999999999995)
32. ('NOLLE', [0.039, 0.315, 0.087, 0.193, 1.0], 3.701)
33. ('ZOCLE', [0.008, 0.315, 0.043, 0.193, 1.0], 3.701)
34. ('BOLYE', [0.091, 0.315, 0.087, 0.012, 1.0], 3.687)
35. ('CONTE', [0.083, 0.315, 0.126, 0.094, 1.0], 3.681)
36. ('GLOME', [0.051, 0.122, 0.142, 0.059, 1.0], 3.666)
37. ('MOLLE', [0.075, 0.315, 0.087, 0.193, 1.0], 3.666)
38. ('MONDE', [0.075, 0.315, 0.126, 0.075, 1.0], 3.6650000000000005)
39. ('DOUCE', [0.059, 0.315, 0.11, 0.051, 1.0], 3.6650000000000005)
40. ('FLOTE', [0.091, 0.122, 0.142, 0.094, 1.0], 3.6619999999999995)
41. ('MONTE', [0.075, 0.315, 0.126, 0.094, 1.0], 3.657)
42. ('FONGE', [0.091, 0.315, 0.126, 0.122, 1.0], 3.654)
43. ('BODGE', [0.091, 0.315, 0.091, 0.122, 1.0], 3.6510000000000002)
44. ('LOGGE', [0.075, 0.315, 0.051, 0.122, 1.0], 3.647)
45. ('OVULE', [0.028, 0.012, 0.11, 0.193, 1.0], 3.6389999999999993)
46. ('HOLWE', [0.051, 0.315, 0.087, 0.008, 1.0], 3.6350000000000002)
47. ('LODDE', [0.075, 0.315, 0.091, 0.075, 1.0], 3.6270000000000002)
48. ('FONDE', [0.091, 0.315, 0.126, 0.075, 1.0], 3.6180000000000003)
49. ('TOGUE', [0.063, 0.315, 0.051, 0.047, 1.0], 3.6150000000000007)
50. ('COGUE', [0.083, 0.315, 0.051, 0.047, 1.0], 3.6150000000000007)
51. ('WHOLE', [0.039, 0.067, 0.142, 0.193, 1.0], 3.615)
52. ('GLOVE', [0.051, 0.122, 0.142, 0.059, 1.0], 3.6109999999999998)
53. ('GLOBE', [0.051, 0.122, 0.142, 0.024, 1.0], 3.6079999999999997)
54. ('CLOVE', [0.083, 0.122, 0.142, 0.059, 1.0], 3.6069999999999998)
55. ('PODGE', [0.063, 0.315, 0.091, 0.122, 1.0], 3.603)
56. ('FOLWE', [0.091, 0.315, 0.087, 0.008, 1.0], 3.596)
57. ('LUNGE', [0.075, 0.11, 0.126, 0.122, 1.0], 3.595)
58. ('PLOCE', [0.063, 0.122, 0.142, 0.051, 1.0], 3.5909999999999997)
59. ('BONCE', [0.091, 0.315, 0.126, 0.051, 1.0], 3.587)
60. ('BOGUE', [0.091, 0.315, 0.051, 0.047, 1.0], 3.5840000000000005)
61. ('DOUPE', [0.059, 0.315, 0.11, 0.028, 1.0], 3.583)
62. ('COUPE', [0.083, 0.315, 0.11, 0.028, 1.0], 3.56)
63. ('ODYLE', [0.028, 0.008, 0.055, 0.193, 1.0], 3.552)
64. ('WOLLE', [0.039, 0.315, 0.087, 0.193, 1.0], 3.548)
65. ('HOUVE', [0.051, 0.315, 0.11, 0.059, 1.0], 3.547)
66. ('CLOKE', [0.083, 0.122, 0.142, 0.024, 1.0], 3.533)
67. ('THULE', [0.063, 0.067, 0.11, 0.193, 1.0], 3.524)
68. ('GLOZE', [0.051, 0.122, 0.142, 0.028, 1.0], 3.521)
69. ('ELOGE', [0.087, 0.122, 0.142, 0.122, 1.0], 3.5209999999999995)
70. ('BUGLE', [0.091, 0.11, 0.051, 0.193, 1.0], 3.513)
71. ('GOUGE', [0.051, 0.315, 0.11, 0.122, 1.0], 3.493)
72. ('TOUZE', [0.063, 0.315, 0.11, 0.028, 1.0], 3.4890000000000003)
73. ('VOGUE', [0.024, 0.315, 0.051, 0.047, 1.0], 3.4850000000000003)
74. ('BULGE', [0.091, 0.11, 0.087, 0.122, 1.0], 3.4779999999999998)
75. ('FUGLE', [0.091, 0.11, 0.051, 0.193, 1.0], 3.473)
76. ('GUYLE', [0.051, 0.11, 0.055, 0.193, 1.0], 3.465)
77. ('MOCHE', [0.075, 0.315, 0.043, 0.055, 1.0], 3.4600000000000004)
78. ('OUNCE', [0.028, 0.11, 0.126, 0.051, 1.0], 3.4530000000000003)
79. ('BOWGE', [0.091, 0.315, 0.031, 0.122, 1.0], 3.446)
80. ('DUPLE', [0.059, 0.11, 0.02, 0.193, 1.0], 3.441)
81. ('BONZE', [0.091, 0.315, 0.126, 0.028, 1.0], 3.434)
82. ('GLUME', [0.051, 0.122, 0.11, 0.059, 1.0], 3.4330000000000003)
83. ('FLUTE', [0.091, 0.122, 0.11, 0.094, 1.0], 3.429)
84. ('DODGE', [0.059, 0.315, 0.091, 0.122, 1.0], 3.426)
85. ('LOVEE', [0.075, 0.315, 0.008, 0.039, 1.0], 3.4259999999999997)
86. ('DULCE', [0.059, 0.11, 0.087, 0.051, 1.0], 3.4250000000000003)
87. ('DONEE', [0.059, 0.315, 0.126, 0.039, 1.0], 3.4170000000000003)
88. ('LOFFE', [0.075, 0.315, 0.004, 0.004, 1.0], 3.4139999999999997)
89. ('BOWNE', [0.091, 0.315, 0.031, 0.067, 1.0], 3.4100000000000006)
90. ('UNCLE', [0.016, 0.028, 0.043, 0.193, 1.0], 3.4060000000000006)
91. ('CHODE', [0.083, 0.067, 0.142, 0.075, 1.0], 3.4020000000000006)
92. ('OBOLE', [0.028, 0.004, 0.142, 0.193, 1.0], 3.3989999999999996)
93. ('COQUE', [0.083, 0.315, 0.012, 0.047, 1.0], 3.3950000000000005)
94. ('TOQUE', [0.063, 0.315, 0.012, 0.047, 1.0], 3.3950000000000005)
95. ('TONNE', [0.063, 0.315, 0.126, 0.067, 1.0], 3.394)
96. ('COMBE', [0.083, 0.315, 0.016, 0.024, 1.0], 3.371)
97. ('YOUZE', [0.008, 0.315, 0.11, 0.028, 1.0], 3.363)
98. ('BONNE', [0.091, 0.315, 0.126, 0.067, 1.0], 3.363)
99. ('NONCE', [0.039, 0.315, 0.126, 0.051, 1.0], 3.362)
100. ('FLUME', [0.091, 0.122, 0.11, 0.059, 1.0], 3.358)
101. ('PLUME', [0.063, 0.122, 0.11, 0.059, 1.0], 3.35)
102. ('GNOME', [0.051, 0.028, 0.142, 0.059, 1.0], 3.3430000000000004)
103. ('ELOPE', [0.087, 0.122, 0.142, 0.028, 1.0], 3.3319999999999994)
104. ('DOWVE', [0.059, 0.315, 0.031, 0.059, 1.0], 3.3300000000000005)
105. ('PHONE', [0.063, 0.067, 0.142, 0.067, 1.0], 3.3230000000000004)
106. ('CHYLE', [0.083, 0.067, 0.055, 0.193, 1.0], 3.3230000000000004)
107. ('FONNE', [0.091, 0.315, 0.126, 0.067, 1.0], 3.323)
108. ('QUOTE', [0.016, 0.11, 0.142, 0.094, 1.0], 3.32)
109. ('CULPE', [0.083, 0.11, 0.087, 0.028, 1.0], 3.32)
110. ('MOTTE', [0.075, 0.315, 0.063, 0.094, 1.0], 3.303)
111. ('KONZE', [0.028, 0.315, 0.126, 0.028, 1.0], 3.3000000000000003)
112. ('NUDGE', [0.039, 0.11, 0.091, 0.122, 1.0], 3.287000000000001)
113. ('TULLE', [0.063, 0.11, 0.087, 0.193, 1.0], 3.284)
114. ('HOWVE', [0.051, 0.315, 0.031, 0.059, 1.0], 3.2750000000000004)
115. ('UNKLE', [0.016, 0.028, 0.012, 0.193, 1.0], 3.2650000000000006)
116. ('FULBE', [0.091, 0.11, 0.087, 0.024, 1.0], 3.2649999999999997)
117. ('UMBLE', [0.016, 0.016, 0.016, 0.193, 1.0], 3.257)
118. ('MELOE', [0.075, 0.236, 0.087, 0.008, 1.0], 3.253)
119. ('ELUDE', [0.087, 0.122, 0.11, 0.075, 1.0], 3.2520000000000002)
120. ('FUNGE', [0.091, 0.11, 0.126, 0.122, 1.0], 3.248)
121. ('BUDGE', [0.091, 0.11, 0.091, 0.122, 1.0], 3.2450000000000006)
122. ('HUDGE', [0.051, 0.11, 0.091, 0.122, 1.0], 3.2440000000000007)
123. ('PHYLE', [0.063, 0.067, 0.055, 0.193, 1.0], 3.244)
124. ('ELUTE', [0.087, 0.122, 0.11, 0.094, 1.0], 3.2439999999999998)
125. ('HUNTE', [0.051, 0.11, 0.126, 0.094, 1.0], 3.2430000000000003)
126. ('OUPHE', [0.028, 0.11, 0.02, 0.055, 1.0], 3.237)
127. ('DUNCE', [0.059, 0.11, 0.126, 0.051, 1.0], 3.2350000000000008)
128. ('FLUKE', [0.091, 0.122, 0.11, 0.024, 1.0], 3.229)
129. ('FLYTE', [0.091, 0.122, 0.055, 0.094, 1.0], 3.2279999999999998)
130. ('FUDGE', [0.091, 0.11, 0.091, 0.122, 1.0], 3.2050000000000005)
131. ('EMULE', [0.087, 0.016, 0.11, 0.193, 1.0], 3.2009999999999996)
132. ('CHOKE', [0.083, 0.067, 0.142, 0.024, 1.0], 3.1940000000000004)
133. ('MEDLE', [0.075, 0.236, 0.091, 0.193, 1.0], 3.1930000000000005)
134. ('LYTHE', [0.075, 0.047, 0.063, 0.055, 1.0], 3.1850000000000005)
135. ('MOEVE', [0.075, 0.315, 0.106, 0.059, 1.0], 3.177)
136. ('POMME', [0.063, 0.315, 0.016, 0.059, 1.0], 3.177)
137. ('LEDGE', [0.075, 0.236, 0.091, 0.122, 1.0], 3.1740000000000004)
138. ('HOOVE', [0.051, 0.315, 0.142, 0.059, 1.0], 3.169)
139. ('ENGLE', [0.087, 0.028, 0.051, 0.193, 1.0], 3.1660000000000004)
140. ('GEODE', [0.051, 0.236, 0.142, 0.075, 1.0], 3.1660000000000004)
141. ('ENODE', [0.087, 0.028, 0.142, 0.075, 1.0], 3.1620000000000004)
142. ('CHUTE', [0.083, 0.067, 0.11, 0.094, 1.0], 3.1610000000000005)
143. ('MYOPE', [0.075, 0.047, 0.142, 0.028, 1.0], 3.154)
144. ('LYCHE', [0.075, 0.047, 0.043, 0.055, 1.0], 3.1450000000000005)
145. ('NONNE', [0.039, 0.315, 0.126, 0.067, 1.0], 3.138)
146. ('GLEDE', [0.051, 0.122, 0.106, 0.075, 1.0], 3.1340000000000003)
147. ('QUOKE', [0.016, 0.11, 0.142, 0.024, 1.0], 3.12)
148. ('BOOZE', [0.091, 0.315, 0.142, 0.028, 1.0], 3.08)
149. ('CYCLE', [0.083, 0.047, 0.043, 0.193, 1.0], 3.075)
150. ('MELNE', [0.075, 0.236, 0.087, 0.067, 1.0], 3.0710000000000006)
151. ('PLENE', [0.063, 0.122, 0.106, 0.067, 1.0], 3.051)
152. ('FLETE', [0.091, 0.122, 0.106, 0.094, 1.0], 3.0509999999999997)
153. ('PLETE', [0.063, 0.122, 0.106, 0.094, 1.0], 3.0429999999999997)
154. ('JUDGE', [0.008, 0.11, 0.091, 0.122, 1.0], 3.0400000000000005)
155. ('COOEE', [0.083, 0.315, 0.142, 0.039, 1.0], 3.04)
156. ('KOPJE', [0.028, 0.315, 0.02, 0.004, 1.0], 3.025)
157. ('EPODE', [0.087, 0.004, 0.142, 0.075, 1.0], 3.024)
158. ('LETHE', [0.075, 0.236, 0.063, 0.055, 1.0], 3.0160000000000005)
159. ('DEKLE', [0.059, 0.236, 0.012, 0.193, 1.0], 3.0040000000000004)
160. ('GLEBE', [0.051, 0.122, 0.106, 0.024, 1.0], 2.997)
161. ('WOWKE', [0.039, 0.315, 0.031, 0.024, 1.0], 2.9850000000000003)
162. ('DELVE', [0.059, 0.236, 0.087, 0.059, 1.0], 2.9840000000000004)
163. ('FLEME', [0.091, 0.122, 0.106, 0.059, 1.0], 2.98)
164. ('CLEPE', [0.083, 0.122, 0.106, 0.028, 1.0], 2.977)
165. ('LECHE', [0.075, 0.236, 0.043, 0.055, 1.0], 2.9760000000000004)
166. ('OZONE', [0.028, 0.004, 0.142, 0.067, 1.0], 2.9530000000000003)
167. ('WELTE', [0.039, 0.236, 0.087, 0.094, 1.0], 2.9450000000000003)
168. ('EMOVE', [0.087, 0.016, 0.142, 0.059, 1.0], 2.945)
169. ('WEYLE', [0.039, 0.236, 0.055, 0.193, 1.0], 2.9410000000000003)
170. ('EXODE', [0.087, 0.012, 0.142, 0.075, 1.0], 2.93)
171. ('HELVE', [0.051, 0.236, 0.087, 0.059, 1.0], 2.9290000000000003)
172. ('MENGE', [0.075, 0.236, 0.126, 0.122, 1.0], 2.9170000000000003)
173. ('LYCEE', [0.075, 0.047, 0.043, 0.039, 1.0], 2.9170000000000003)
174. ('NEELE', [0.039, 0.236, 0.106, 0.193, 1.0], 2.9170000000000003)
175. ('PLEBE', [0.063, 0.122, 0.106, 0.024, 1.0], 2.9139999999999997)
176. ('ETTLE', [0.087, 0.012, 0.063, 0.193, 1.0], 2.906)
177. ('TEDGE', [0.063, 0.236, 0.091, 0.122, 1.0], 2.8980000000000006)
178. ('MEUTE', [0.075, 0.236, 0.11, 0.094, 1.0], 2.8970000000000002)
179. ('BUTTE', [0.091, 0.11, 0.063, 0.094, 1.0], 2.89)
180. ('THYME', [0.063, 0.067, 0.055, 0.059, 1.0], 2.8890000000000007)
181. ('CHYME', [0.083, 0.067, 0.055, 0.059, 1.0], 2.8890000000000007)
182. ('MYTHE', [0.075, 0.047, 0.063, 0.055, 1.0], 2.8850000000000007)
183. ('UNDUE', [0.016, 0.028, 0.091, 0.047, 1.0], 2.882000000000001)
184. ('ENDUE', [0.087, 0.028, 0.091, 0.047, 1.0], 2.882000000000001)
185. ('DEUCE', [0.059, 0.236, 0.11, 0.051, 1.0], 2.8810000000000007)
186. ('ETUDE', [0.087, 0.012, 0.11, 0.075, 1.0], 2.8780000000000006)
187. ('BELLE', [0.091, 0.236, 0.087, 0.193, 1.0], 2.875)
188. ('HENDE', [0.051, 0.236, 0.126, 0.075, 1.0], 2.8730000000000007)
189. ('ZUCHE', [0.008, 0.11, 0.043, 0.055, 1.0], 2.8730000000000007)
190. ('HEDGE', [0.051, 0.236, 0.091, 0.122, 1.0], 2.8660000000000005)
191. ('ECCLE', [0.087, 0.004, 0.043, 0.193, 1.0], 2.866)
192. ('LEGGE', [0.075, 0.236, 0.051, 0.122, 1.0], 2.863)
193. ('EDUCE', [0.087, 0.008, 0.11, 0.051, 1.0], 2.8300000000000005)
194. ('LEEDE', [0.075, 0.236, 0.106, 0.075, 1.0], 2.8270000000000004)
195. ('PEELE', [0.063, 0.236, 0.106, 0.193, 1.0], 2.827)
196. ('FUGUE', [0.091, 0.11, 0.051, 0.047, 1.0], 2.8230000000000004)
197. ('LETTE', [0.075, 0.236, 0.063, 0.094, 1.0], 2.819)
198. ('EVOKE', [0.087, 0.012, 0.142, 0.024, 1.0], 2.812)
199. ('VENGE', [0.024, 0.236, 0.126, 0.122, 1.0], 2.811)
200. ('HENCE', [0.051, 0.236, 0.126, 0.051, 1.0], 2.8020000000000005)
201. ('VENUE', [0.024, 0.236, 0.126, 0.047, 1.0], 2.7950000000000004)
202. ('ELEME', [0.087, 0.122, 0.106, 0.059, 1.0], 2.795)
203. ('MELEE', [0.075, 0.236, 0.087, 0.039, 1.0], 2.7760000000000002)
204. ('BELEE', [0.091, 0.236, 0.087, 0.039, 1.0], 2.769)
205. ('WYTHE', [0.039, 0.047, 0.063, 0.055, 1.0], 2.767000000000001)
206. ('WENDE', [0.039, 0.236, 0.126, 0.075, 1.0], 2.763000000000001)
207. ('FENCE', [0.091, 0.236, 0.126, 0.051, 1.0], 2.7630000000000003)
208. ('WEDGE', [0.039, 0.236, 0.091, 0.122, 1.0], 2.7560000000000007)
209. ('PENCE', [0.063, 0.236, 0.126, 0.051, 1.0], 2.7550000000000003)
210. ('LEEME', [0.075, 0.236, 0.106, 0.059, 1.0], 2.748)
211. ('KYTHE', [0.028, 0.047, 0.063, 0.055, 1.0], 2.7440000000000007)
212. ('ELEVE', [0.087, 0.122, 0.106, 0.059, 1.0], 2.7399999999999998)
213. ('KEDGE', [0.028, 0.236, 0.091, 0.122, 1.0], 2.7330000000000005)
214. ('PEKOE', [0.063, 0.236, 0.012, 0.008, 1.0], 2.729)
215. ('TEYNE', [0.063, 0.236, 0.055, 0.067, 1.0], 2.7280000000000006)
216. ('THEME', [0.063, 0.067, 0.106, 0.059, 1.0], 2.7120000000000006)
217. ('PHENE', [0.063, 0.067, 0.106, 0.067, 1.0], 2.7120000000000006)
218. ('MEYNE', [0.075, 0.236, 0.055, 0.067, 1.0], 2.7040000000000006)
219. ('EXUDE', [0.087, 0.012, 0.11, 0.075, 1.0], 2.6970000000000005)
220. ('HEYNE', [0.051, 0.236, 0.055, 0.067, 1.0], 2.6960000000000006)
221. ('TUQUE', [0.063, 0.11, 0.012, 0.047, 1.0], 2.6740000000000004)
222. ('BEDYE', [0.091, 0.236, 0.091, 0.012, 1.0], 2.6700000000000004)
223. ('BECHE', [0.091, 0.236, 0.043, 0.055, 1.0], 2.6690000000000005)
224. ('FEYNE', [0.091, 0.236, 0.055, 0.067, 1.0], 2.6570000000000005)
225. ('CHEVE', [0.083, 0.067, 0.106, 0.059, 1.0], 2.6570000000000005)
226. ('OXEYE', [0.028, 0.012, 0.106, 0.012, 1.0], 2.655)
227. ('TYTHE', [0.063, 0.047, 0.063, 0.055, 1.0], 2.6530000000000005)
228. ('HYTHE', [0.051, 0.047, 0.063, 0.055, 1.0], 2.6530000000000005)
229. ('LEVEE', [0.075, 0.236, 0.008, 0.039, 1.0], 2.642)
230. ('FYTTE', [0.091, 0.047, 0.063, 0.094, 1.0], 2.641)
231. ('QUEME', [0.016, 0.11, 0.106, 0.059, 1.0], 2.6380000000000003)
232. ('TENNE', [0.063, 0.236, 0.126, 0.067, 1.0], 2.6100000000000003)
233. ('EMPTE', [0.087, 0.016, 0.02, 0.094, 1.0], 2.594)
234. ('BENNE', [0.091, 0.236, 0.126, 0.067, 1.0], 2.579)
235. ('PHEBE', [0.063, 0.067, 0.106, 0.024, 1.0], 2.575)
236. ('KYDDE', [0.028, 0.047, 0.091, 0.075, 1.0], 2.5710000000000006)
237. ('DETTE', [0.059, 0.236, 0.063, 0.094, 1.0], 2.5660000000000003)
238. ('HEGGE', [0.051, 0.236, 0.051, 0.122, 1.0], 2.555)
239. ('NETTE', [0.039, 0.236, 0.063, 0.094, 1.0], 2.5540000000000003)
240. ('VEHME', [0.024, 0.236, 0.004, 0.059, 1.0], 2.519)
241. ('METTE', [0.075, 0.236, 0.063, 0.094, 1.0], 2.519)
242. ('FETTE', [0.091, 0.236, 0.063, 0.094, 1.0], 2.472)
243. ('WEYVE', [0.039, 0.236, 0.055, 0.059, 1.0], 2.4520000000000004)
244. ('QUEUE', [0.016, 0.11, 0.106, 0.047, 1.0], 2.422)
245. ('EVENE', [0.087, 0.012, 0.106, 0.067, 1.0], 2.4090000000000003)
246. ('KEMPE', [0.028, 0.236, 0.016, 0.028, 1.0], 2.406)
247. ('FEMME', [0.091, 0.236, 0.016, 0.059, 1.0], 2.4010000000000002)
248. ('PEECE', [0.063, 0.236, 0.106, 0.051, 1.0], 2.4010000000000002)
249. ('TEPEE', [0.063, 0.236, 0.02, 0.039, 1.0], 2.39)
250. ('BEEVE', [0.091, 0.236, 0.106, 0.059, 1.0], 2.386)
251. ('ETWEE', [0.087, 0.012, 0.031, 0.039, 1.0], 2.3110000000000004)
252. ('PEWEE', [0.063, 0.236, 0.031, 0.039, 1.0], 2.2830000000000004)
253. ('FEEZE', [0.091, 0.236, 0.106, 0.028, 1.0], 2.2560000000000002)
254. ('KEEVE', [0.028, 0.236, 0.106, 0.059, 1.0], 2.2520000000000002)

LODGE: guess #2
OBOBG: hint #2
From 254 words to 5 words in 0.004 seconds.
Counted word list letters, sorted by frequency in 0.004687001999997165 seconds.
Letters ranked by likelihood of single appearance in word list:
'D' frequency, positional: [0.8, 0.0, 0.0, 0.2, 0.0], by letter: 0.2, by word appearance: 1.0
'E' frequency, positional: [0.2, 0.4, 0.0, 0.0, 1.0], by letter: 0.32, by word appearance: 1.0
'L' frequency, positional: [0.0, 0.2, 0.4, 0.4, 0.0], by letter: 0.2, by word appearance: 1.0
'U' frequency, positional: [0.0, 0.4, 0.2, 0.0, 0.0], by letter: 0.12, by word appearance: 0.6
'C' frequency, positional: [0.0, 0.0, 0.0, 0.2, 0.0], by letter: 0.04, by word appearance: 0.2
'K' frequency, positional: [0.0, 0.0, 0.2, 0.0, 0.0], by letter: 0.04, by word appearance: 0.2
'P' frequency, positional: [0.0, 0.0, 0.2, 0.0, 0.0], by letter: 0.04, by word appearance: 0.2
'V' frequency, positional: [0.0, 0.0, 0.0, 0.2, 0.0], by letter: 0.04, by word appearance: 0.2
'A' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'B' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'F' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'G' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'H' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'I' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'J' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'M' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'N' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'O' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'Q' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'R' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'S' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'T' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'W' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'X' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'Y' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'Z' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0

Words ranked by sum of each letter positional frequency + word appearance frequency (each unique letter single count, so repeat letters don't add) in 0.0005159999999762022 seconds.
Words ranked:
1. ('DUPLE', [0.8, 0.4, 0.2, 0.4, 1.0], 6.6000000000000005)
2. ('DULCE', [0.8, 0.4, 0.4, 0.2, 1.0], 6.6000000000000005)
3. ('DELVE', [0.8, 0.4, 0.4, 0.2, 1.0], 5.6000000000000005)
4. ('DEKLE', [0.8, 0.4, 0.2, 0.4, 1.0], 5.6000000000000005)
5. ('ELUDE', [0.2, 0.2, 0.2, 0.2, 1.0], 5.2)

DELVE: guess #3
OOOBG: hint #3
From 5 words to 1 words in 0.0 seconds.
Counted word list letters, sorted by frequency in 0.0037037939999891023 seconds.
Letters ranked by likelihood of single appearance in word list:
'D' frequency, positional: [0.0, 0.0, 0.0, 1.0, 0.0], by letter: 0.2, by word appearance: 1.0
'E' frequency, positional: [1.0, 0.0, 0.0, 0.0, 1.0], by letter: 0.4, by word appearance: 1.0
'L' frequency, positional: [0.0, 1.0, 0.0, 0.0, 0.0], by letter: 0.2, by word appearance: 1.0
'U' frequency, positional: [0.0, 0.0, 1.0, 0.0, 0.0], by letter: 0.2, by word appearance: 1.0
'A' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'B' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'C' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'F' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'G' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'H' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'I' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'J' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'K' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'M' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'N' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'O' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'P' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'Q' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'R' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'S' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'T' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'V' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'W' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'X' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'Y' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0
'Z' frequency, positional: [0.0, 0.0, 0.0, 0.0, 0.0], by letter: 0.0, by word appearance: 0.0

Words ranked by sum of each letter positional frequency + word appearance frequency (each unique letter single count, so repeat letters don't add) in 0.0005677990000094724 seconds.
Words ranked:
1. ('ELUDE', [1.0, 1.0, 1.0, 1.0, 1.0], 8.0)

