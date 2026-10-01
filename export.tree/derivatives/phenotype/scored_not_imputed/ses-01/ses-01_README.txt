Please read this README.txt file before utilising the TSV data for this session from the PsiConnect study. This document contains critical methodological amendments that directly impact psychometric interpretation and statistical analysis. JSON files provide additional information about each measure, including wording of items and their presentation. It also contains information as to how subscales were derived and references for each measure.

Self-Compassion Scale (SCS)
- 7-point scale incorrectly implemented instead of standard 5-point Likert
- Participants instructed to use only middle 5 columns, ignoring leftmost and rightmost
- Some versions had end columns labelled with "---" for clarity
- Note: Response inconsistency may exist across participants
- Raw shows this version
- Recoded suffix has the following recoding provided:

1. No transformation:
   - Applied when responses are already on a 1-5 scale
   - No changes are made to the original values

2. Linear shift:
   - Applied when responses are outside the 1-5 range
   - Applied to scales with exactly 4 or 5 contiguous values (e.g., 3-6, 2-6)
   - Original values are linearly mapped to the 1-5 scale
   - Formula: new_value = 1 + (original_value - min_value) * (4 / (max_value - min_value))
   - Example: if responses are on a 3-6 scale, 3→1, 4→2.33, 5→3.67, 6→5

3. Discrete remapping:
   - Applied when responses span 6 or more numbers (typically a 1-7 or 2-7 scale)
   - Values are mapped according to the following scheme:
     * 1 → 1
     * 2-3 → 2
     * 4 → 3
     * 5-6 → 4
     * 7+ → 5

Total participants processed: 66
Total participants transformed: 64
Discrete remapping participants: 47
Linear shift participants: 17

participant_id	transformation_applied	original_values	recoded_values
PC001	discrete remapping	3 2 4 2 3 6 3 4 3 3 3 2 3 2 7 2 4 2 3 2 2 3 6 7 4 3	2 2 3 2 2 4 2 3 2 2 2 2 2 2 5 2 3 2 2 2 2 2 4 5 3 2
PC002	discrete remapping	1 6 2 7 4 6 3 7 4 4 7 4 7 4 4 7 4 7 4 6 7 4 3 7 7 4	1 4 2 5 3 4 2 5 3 3 5 3 5 3 3 5 3 5 3 4 5 3 2 5 5 3
PC003	discrete remapping	2 7 5 1 7 7 3 7 3 3 7 6 7 4 3 1 3 7 6 2 7 6 4 1 7 3	2 5 4 1 5 5 2 5 2 2 5 4 5 3 2 1 2 5 4 2 5 4 3 1 5 2
PC004	no valid responses	N/A	N/A
PC005	discrete remapping	7 7 2 7 6 6 3 7 6 6 7 2 7 2 4 7 3 7 3 6 7 2 3 6 2 2	5 5 2 5 4 4 2 5 4 4 5 2 5 2 3 5 2 5 2 4 5 2 2 4 2 2
PC006	discrete remapping	2 6 4 7 4 7 3 4 5 2 6 3 7 5 5 6 5 7 4 1 6 4 4 1 7 4	2 4 3 5 3 5 2 3 4 2 4 2 5 4 4 4 4 5 3 1 4 3 3 1 5 3
PC007	linear shift	3 2 2 4 6 2 6 2 2 2 6 2 6 2 2 2 6 6 6 3 2 2 2 2 6 6	2 1 1 3 5 1 5 1 1 1 5 1 5 1 1 1 5 5 5 2 1 1 1 1 5 5
PC008	discrete remapping	4 2 3 3 3 3 7 3 2 2 2 2 2 3 2 2 3 2 3 2 7 5 2 6 4 2	3 2 2 2 2 2 5 2 2 2 2 2 2 2 2 2 2 2 2 2 5 4 2 4 3 2
PC009	linear shift	3 6 3 4 2 3 3 6 2 3 3 6 6 3 3 6 3 6 6 3 3 3 3 6 6 3	2 5 2 3 1 2 2 5 1 2 2 5 5 2 2 5 2 5 5 2 2 2 2 5 5 2
PC010	discrete remapping	2 6 2 2 3 2 3 6 4 4 3 3 7 3 5 7 3 2 3 6 6 3 3 2 6 3	2 4 2 2 2 2 2 4 3 3 2 2 5 2 4 5 2 2 2 4 4 2 2 2 4 2
PC011	discrete remapping	2 6 2 6 1 6 6 1 6 6 7 7 6 6 3 2 6 6 6 7 7 6 6 7 7 6	2 4 2 4 1 4 4 1 4 4 5 5 4 4 2 2 4 4 4 5 5 4 4 5 5 4
PC012	discrete remapping	6 6 4 6 2 7 4 2 4 4 7 3 7 4 4 6 4 7 3 7 2 3 3 7 7 3	4 4 3 4 2 5 3 2 3 3 5 2 5 3 3 4 3 5 2 5 2 2 2 5 5 2
PC013	discrete remapping	3 4 4 2 4 6 4 6 5 7 7 3 7 4 3 6 3 1 3 1 6 4 3 2 3 2	2 3 3 2 3 4 3 4 4 5 5 2 5 3 2 4 2 1 2 1 4 3 2 2 2 2
PC014	discrete remapping	6 6 4 2 3 6 3 6 3 2 7 3 2 4 3 7 4 2 3 6 6 3 3 7 6 3	4 4 3 2 2 4 2 4 2 2 5 2 2 3 2 5 3 2 2 4 4 2 2 5 4 2
PC015	discrete remapping	6 2 6 3 2 2 4 6 4 3 7 3 6 4 3 6 3 7 3 6 7 2 3 2 6 3	4 2 4 2 2 2 3 4 3 2 5 2 4 3 2 4 2 5 2 4 5 2 2 2 4 2
PC016	discrete remapping	7 7 6 7 2 6 7 6 2 7 2 6 6 6 7 6 2 6 2 6 7 6 6 7 7 6	5 5 4 5 2 4 5 4 2 5 2 4 4 4 5 4 2 4 2 4 5 4 4 5 5 4
PC017	linear shift	2 6 3 6 3 6 3 2 3 2 6 2 2 3 3 3 3 2 3 6 6 3 3 6 2 2	1 5 2 5 2 5 2 1 2 1 5 1 1 2 2 2 2 1 2 5 5 2 2 5 1 1
PC018	discrete remapping	2 6 4 2 4 6 6 6 3 3 7 4 7 4 5 6 3 7 4 6 7 5 4 7 6 3	2 4 3 2 3 4 4 4 2 2 5 3 5 3 4 4 2 5 3 4 5 4 3 5 4 2
PC019	linear shift	6 2 2 2 3 6 3 3 2 6 6 6 2 6 3 6 3 3 2 3 3 3 3 2 3 3	5 1 1 1 2 5 2 2 1 5 5 5 1 5 2 5 2 2 1 2 2 2 2 1 2 2
PC020	linear shift	7 7 3 7 4 7 3 7 4 3 7 4 7 4 4 7 4 7 4 7 7 4 4 7 6 4	5 5 1 5 2 5 1 5 2 1 5 2 5 2 2 5 2 5 2 5 5 2 2 5 4 2
PC021	linear shift	3 2 2 2 6 3 6 3 3 6 3 2 6 3 6 3 3 2 2 3 3 2 2 2 3 2	2 1 1 1 5 2 5 2 2 5 2 1 5 2 5 2 2 1 1 2 2 1 1 1 2 1
PC022	linear shift	3 3 4 6 3 6 4 3 3 4 6 3 3 2 3 2 3 2 2 3 3 3 2 6 3 2	2 2 3 5 2 5 3 2 2 3 5 2 2 1 2 1 2 1 1 2 2 2 1 5 2 1
PC023	linear shift	2 2 3 6 3 6 3 2 3 3 6 3 6 3 3 3 3 6 3 6 6 3 3 6 6 3	1 1 2 5 2 5 2 1 2 2 5 2 5 2 2 2 2 5 2 5 5 2 2 5 5 2
PC024	linear shift	6 6 3 6 3 6 3 3 3 3 6 2 2 3 3 6 6 6 3 2 6 3 3 2 6 6	5 5 2 5 2 5 2 2 2 2 5 1 1 2 2 5 5 5 2 1 5 2 2 1 5 5
PC025	discrete remapping	2 6 3 6 3 2 3 3 3 6 2 6 6 4 3 2 2 6 2 7 2 6 2 2 3 6	2 4 2 4 2 2 2 2 2 4 2 4 4 3 2 2 2 4 2 5 2 4 2 2 2 4
PC026	discrete remapping	3 2 3 3 4 6 4 6 3 4 6 4 7 4 4 6 3 6 4 2 7 3 3 7 3 4	2 2 2 2 3 4 3 4 2 3 4 3 5 3 3 4 2 4 3 2 5 2 2 5 2 3
PC027	discrete remapping	7 7 3 6 2 7 2 7 4 2 6 2 7 5 5 7 4 7 3 2 3 4 4 3 3 4	5 5 2 4 2 5 2 5 3 2 4 2 5 4 4 5 3 5 2 2 2 3 3 2 2 3
PC028	discrete remapping	6 3 2 7 6 6 2 6 2 3 6 2 3 6 3 2 3 3 2 3 2 7 2 3 2 3	4 2 2 5 4 4 2 4 2 2 4 2 2 4 2 2 2 2 2 2 2 5 2 2 2 2
PC029	discrete remapping	6 2 4 2 4 2 6 7 4 2 6 4 7 3 2 2 3 7 4 2 7 3 4 7 3 3	4 2 3 2 3 2 4 5 3 2 4 3 5 2 2 2 2 5 3 2 5 2 3 5 2 2
PC030	discrete remapping	6 7 2 7 4 6 3 2 6 3 7 7 6 4 3 3 3 2 3 7 7 3 3 7 2 2	4 5 2 5 3 4 2 2 4 2 5 5 4 3 2 2 2 2 2 5 5 2 2 5 2 2
PC031	discrete remapping	4 6 6 4 7 2 2 3 3 6 3 6 3 3 3 6 3 7 2 6 4 3 2 6 3 6	3 4 4 3 5 2 2 2 2 4 2 4 2 2 2 4 2 5 2 4 3 2 2 4 2 4
PC032	discrete remapping	3 2 3 4 4 3 3 3 4 3 3 3 3 4 4 3 4 7 3 6 2 3 6 6 2 2	2 2 2 3 3 2 2 2 3 2 2 2 2 3 3 2 3 5 2 4 2 2 4 4 2 2
PC201	discrete remapping	7 6 4 1 4 7 4 7 4 4 1 3 7 4 4 1 4 4 5 7 1 4 4 1 7 5	5 4 3 1 3 5 3 5 3 3 1 2 5 3 3 1 3 3 4 5 1 3 3 1 5 4
PC202	linear shift	3 3 3 4 6 3 3 3 2 4 3 2 2 2 3 3 3 6 6 2 3 3 6 4 3 2	2 2 2 3 5 2 2 2 1 3 2 1 1 1 2 2 2 5 5 1 2 2 5 3 2 1
PC203	discrete remapping	7 6 2 1 4 1 1 3 2 1 7 2 6 2 3 2 3 6 3 3 2 4 2 7 2 6	5 4 2 1 3 1 1 2 2 1 5 2 4 2 2 2 2 4 2 2 2 3 2 5 2 4
PC204	discrete remapping	4 2 3 6 2 2 2 3 3 3 6 2 6 4 3 7 4 6 3 7 3 4 3 6 3 3	3 2 2 4 2 2 2 2 2 2 4 2 4 3 2 5 3 4 2 5 2 3 2 4 2 2
PC205	discrete remapping	7 6 2 7 3 3 2 6 4 2 7 3 6 6 3 6 3 7 3 7 7 2 4 7 3 4	5 4 2 5 2 2 2 4 3 2 5 2 4 4 2 4 2 5 2 5 5 2 3 5 2 3
PC206	linear shift	4 3 2 4 2 4 2 4 3 3 4 2 3 6 2 2 2 3 2 3 3 6 6 6 2 6	3 2 1 3 1 3 1 3 2 2 3 1 2 5 1 1 1 2 1 2 2 5 5 5 1 5
PC207	discrete remapping	3 6 4 2 3 2 3 2 2 6 3 3 7 3 3 6 3 2 3 4 3 3 3 3 7 6	2 4 3 2 2 2 2 2 2 4 2 2 5 2 2 4 2 2 2 3 2 2 2 2 5 4
PC208	discrete remapping	3 7 4 7 3 2 4 3 2 3 2 2 2 3 4 6 4 6 2 3 3 6 3 6 3 3	2 5 3 5 2 2 3 2 2 2 2 2 2 2 3 4 3 4 2 2 2 4 2 4 2 2
PC209	discrete remapping	6 1 5 7 5 3 5 1 4 5 7 4 1 5 5 1 5 7 5 2 1 5 5 7 7 5	4 1 4 5 4 2 4 1 3 4 5 3 1 4 4 1 4 5 4 2 1 4 4 5 5 4
PC210	linear shift	2 3 2 3 6 2 2 3 3 3 2 2 2 2 2 2 2 2 2 3 3 2 2 2 2 2	1 2 1 2 5 1 1 2 2 2 1 1 1 1 1 1 1 1 1 2 2 1 1 1 1 1
PC211	linear shift	4 4 3 3 3 3 2 4 4 2 4 2 2 3 3 3 2 2 6 2 4 2 6 6 4 3	3 3 2 2 2 2 1 3 3 1 3 1 1 2 2 2 1 1 5 1 3 1 5 5 3 2
PC213	discrete remapping	2 3 6 3 3 4 6 3 2 2 2 2 3 2 3 3 3 3 2 3 3 7 7 3 3 6	2 2 4 2 2 3 4 2 2 2 2 2 2 2 2 2 2 2 2 2 2 5 5 2 2 4
PC212	discrete remapping	3 5 3 4 6 4 1 3 4 6 2 6 6 4 4 4 4 2 2 7 3 6 3 1 6 3	2 4 2 3 4 3 1 2 3 4 2 4 4 3 3 3 3 2 2 5 2 4 2 1 4 2
PC214	discrete remapping	2 6 4 7 4 3 5 7 3 5 2 5 1 5 4 7 4 1 5 3 7 2 4 1 1 3	2 4 3 5 3 2 4 5 2 4 2 4 1 4 3 5 3 1 4 2 5 2 3 1 1 2
PC215	discrete remapping	4 4 6 4 2 4 6 4 3 7 3 6 3 2 3 4 6 3 6 3 4 3 7 2 3 2	3 3 4 3 2 3 4 3 2 5 2 4 2 2 2 3 4 2 4 2 3 2 5 2 2 2
PC216	discrete remapping	2 2 4 6 4 7 3 3 2 2 3 2 7 3 4 2 2 2 3 2 6 2 2 7 7 3	2 2 3 4 3 5 2 2 2 2 2 2 5 2 3 2 2 2 2 2 4 2 2 5 5 2
PC217	discrete remapping	2 6 7 7 3 7 3 6 3 7 7 2 2 3 3 6 3 2 2 7 7 3 3 7 6 3	2 4 5 5 2 5 2 4 2 5 5 2 2 2 2 4 2 2 2 5 5 2 2 5 4 2
PC218	discrete remapping	3 3 2 2 6 4 2 3 2 6 3 6 2 6 6 3 2 3 6 4 3 7 2 4 4 6	2 2 2 2 4 3 2 2 2 4 2 4 2 4 4 2 2 2 4 3 2 5 2 3 3 4
PC219	discrete remapping	3 6 4 7 4 7 4 3 2 3 2 3 6 2 3 3 3 6 3 2 6 2 2 6 6 2	2 4 3 5 3 5 3 2 2 2 2 2 4 2 2 2 2 4 2 2 4 2 2 4 4 2
PC220	discrete remapping	6 3 3 2 6 2 3 2 3 3 6 6 7 3 4 6 4 7 2 2 2 2 2 6 2 2	4 2 2 2 4 2 2 2 2 2 4 4 5 2 3 4 3 5 2 2 2 2 2 4 2 2
PC221	linear shift	2 3 3 2 3 2 3 2 3 3 6 3 2 2 3 2 3 2 3 2 6 2 3 2 3 3	1 2 2 1 2 1 2 1 2 2 5 2 1 1 2 1 2 1 2 1 5 1 2 1 2 2
PC222	linear shift	3 6 2 6 2 2 3 3 3 3 2 2 6 4 3 2 3 2 2 6 3 3 4 6 2 2	2 5 1 5 1 1 2 2 2 2 1 1 5 3 2 1 2 1 1 5 2 2 3 5 1 1
PC223	linear shift	3 3 3 6 3 2 2 2 3 2 3 3 6 3 6 2 3 6 2 3 3 2 2 2 3 2	2 2 2 5 2 1 1 1 2 1 2 2 5 2 5 1 2 5 1 2 2 1 1 1 2 1
PC224	discrete remapping	4 3 4 2 2 2 3 3 6 3 4 7 4 2 4 4 2 2 7 4 3 6 6 3 3 6	3 2 3 2 2 2 2 2 4 2 3 5 3 2 3 3 2 2 5 3 2 4 4 2 2 4
PC225	linear shift	6 3 3 2 3 3 3 3 3 3 6 6 6 3 3 3 2 6 2 2 6 3 3 6 6 3	5 2 2 1 2 2 2 2 2 2 5 5 5 2 2 2 1 5 1 1 5 2 2 5 5 2
PC226	discrete remapping	3 2 3 7 3 3 2 3 4 4 2 3 2 4 2 3 4 6 3 6 6 4 2 7 2 2	2 2 2 5 2 2 2 2 3 3 2 2 2 3 2 2 3 4 2 4 4 3 2 5 2 2
PC227	discrete remapping	7 2 3 2 4 6 3 6 3 3 7 3 2 3 4 6 3 2 3 2 6 3 4 6 6 3	5 2 2 2 3 4 2 4 2 2 5 2 2 2 3 4 2 2 2 2 4 2 3 4 4 2
PC228	discrete remapping	6 2 3 7 3 4 3 2 3 2 2 2 2 3 6 6 2 6 3 2 6 3 3 6 3 3	4 2 2 5 2 3 2 2 2 2 2 2 2 2 4 4 2 4 2 2 4 2 2 4 2 2
PC229	discrete remapping	7 7 4 7 4 7 4 2 4 4 6 4 6 4 4 6 4 2 4 6 4 4 3 7 7 4	5 5 3 5 3 5 3 2 3 3 4 3 4 3 3 4 3 2 3 4 3 3 2 5 5 3
PC230	discrete remapping	1 2 4 2 3 7 6 7 3 3 6 4 7 4 4 6 4 7 3 2 7 6 3 6 7 2	1 2 3 2 2 5 4 5 2 2 4 3 5 3 3 4 3 5 2 2 5 4 2 4 5 2
PC231	discrete remapping	3 3 6 3 3 4 2 6 2 2 6 3 6 3 2 4 2 6 4 3 7 2 6 2 3 2	2 2 4 2 2 3 2 4 2 2 4 2 4 2 2 3 2 4 3 2 5 2 4 2 2 2
PC232	discrete remapping	2 2 3 2 3 6 3 2 4 3 6 4 6 4 4 6 4 2 3 2 6 4 3 7 2 4	2 2 2 2 2 4 2 2 3 2 4 3 4 3 3 4 3 2 2 2 4 3 2 5 2 3
PC233	discrete remapping	7 6 4 7 3 6 4 6 4 4 6 4 6 4 3 7 4 2 3 6 6 2 3 6 2 2	5 4 3 5 2 4 3 4 3 3 4 3 4 3 2 5 3 2 2 4 4 2 2 4 2 2

Barcelona Music Reward Questionnaire (BMRQ)
- Scored using factor analysis matrix from Mas-Herrero et al. 2013
- These factors may not perfectly apply to different populations/cultures

Inventory of Depression and Anxiety Symptoms (IDAS-II)
- Analysis constrained to 34 specific items:
  a) 26 core items (2,3,5,7,8,9,10,16,21,23,27,31,32,39,40,45,48,49,50,53,56,57,58,59,61,64)
  b) 8 additional items (1,6,11,13,26,30,51,52)
- Constructs four subscales:
  a) Dysphoria (10 items): marker of anxiety & depression
  b) Well-Being (8 items): specific to depression
  c) Panic (8 items): specific to anxiety
  d) General Depression (20 items): broader construct coverage