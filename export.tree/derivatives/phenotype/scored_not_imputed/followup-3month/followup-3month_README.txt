Please read this README.txt file before utilising the TSV data for this session from the PsiConnect study. This document contains critical methodological amendments that directly impact psychometric interpretation and statistical analysis. JSON files provide additional information about each measure, including wording of items and their presentation. It also contains information as to how subscales were derived and references for each measure.

Self-Compassion Scale (SCS)
- 7-point scale incorrectly implemented instead of standard 5-point Likert
- Participants instructed to use only middle 5 columns, ignoring leftmost and rightmost
- Some versions had end columns labelled with "---" for clarity
- Note: Response inconsistency 5 exist across participants
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

Total participants processed: 56
Total participants transformed: 54
Discrete remapping participants: 11
Linear shift participants: 43

participant_id	original_scale	transformation_applied	original_values
PC001	3-7	linear shift	5 5 6 6 6 7 5 6 6 5 4 6 4 5 5 6 3 6 6 5 6 6 5 4 7 6
PC002	2-6	linear shift	2 2 6 2 6 2 6 2 6 6 2 6 2 6 6 2 6 2 6 2 2 6 6 2 2 6
PC003	1-6	discrete remapping	4 2 6 1 5 2 6 3 6 5 5 5 2 6 5 2 6 2 5 2 2 4 6 1 2 6
PC004	2-6	linear shift	5 5 3 4 4 5 3 4 3 3 5 4 4 4 4 5 3 4 4 6 3 2 3 5 5 3
PC005	2-6	linear shift	2 2 2 2 2 2 2 2 6 6 6 6 6 6 6 6 6 6 6 6 6 6 6 6 4 4
PC006	1-7	discrete remapping	4 3 5 4 6 4 4 4 6 4 3 5 3 7 5 3 6 4 6 5 3 3 6 1 3 6
PC007	3-6	linear shift	6 4 4 6 3 5 5 5 4 5 5 3 3 4 4 5 4 3 4 5 4 5 3 4 4 4
PC008	4-6	linear shift	5 5 6 6 5 5 4 5 6 5 6 5 4 6 6 4 5 6 6 5 4 6 5 5 5 5
PC009	2-5	linear shift	3 4 4 3 4 5 4 3 4 5 2 4 4 4 5 5 5 4 4 5 3 4 5 3 4 5
PC010	3-6	linear shift	4 3 5 3 5 4 5 4 6 5 4 5 4 5 5 5 5 3 5 3 4 5 4 3 3 5
PC012	1-7	discrete remapping	2 2 6 2 6 1 6 4 7 7 5 7 2 7 5 3 6 2 6 2 5 6 6 1 2 6
PC013	1-7	discrete remapping	2 1 5 2 6 1 2 1 7 4 2 6 1 5 5 2 5 2 6 1 2 5 6 1 2 6
PC015	2-6	linear shift	2 3 4 2 5 4 4 3 4 4 4 5 2 4 4 2 5 2 6 4 2 3 5 3 4 5
PC016	3-5	linear shift	4 4 5 5 4 5 4 4 3 4 4 4 3 3 4 4 4 5 3 5 5 4 4 4 4 4
PC017	2-6	linear shift	5 2 6 2 5 2 6 3 5 5 2 5 2 6 6 4 6 3 5 2 2 6 6 2 5 5
PC018	2-6	linear shift	3 3 5 3 5 5 4 4 6 5 4 5 2 6 6 3 6 2 5 4 3 6 6 3 4 5
PC019	3-6	linear shift	3 5 5 3 5 3 4 5 3 5 3 4 4 4 5 3 5 4 5 5 5 5 3 5 6 5
PC020	2-6	linear shift	2 2 6 3 6 2 6 2 6 6 2 6 4 6 6 2 6 4 6 2 2 6 6 2 5 5
PC021	2-6	linear shift	4 3 5 3 5 2 3 4 6 5 3 5 2 5 5 3 5 3 5 3 3 6 5 2 3 5
PC022	2-6	linear shift	4 4 6 3 6 4 6 4 5 6 3 5 3 5 6 4 6 2 5 4 3 5 6 5 4 6
PC023	3-5	linear shift	4 3 5 3 5 3 5 3 5 5 3 5 3 5 5 3 5 3 5 3 3 5 5 3 4 5
PC025	3-6	linear shift	4 4 4 6 3 3 3 4 6 3 3 5 4 5 5 5 5 5 5 5 5 3 4 3 5 4
PC026	2-6	linear shift	2 3 5 3 6 2 5 3 6 6 2 6 2 6 6 3 6 4 6 5 2 6 5 2 5 6
PC027	2-6	linear shift	2 2 6 2 5 2 4 2 5 5 2 5 2 6 6 2 5 3 5 3 3 6 6 3 4 6
PC028	3-6	linear shift	4 6 4 5 4 5 4 3 4 4 5 4 4 4 5 5 4 4 4 5 5 4 4 5 4 4
PC029	3-6	linear shift	4 5 6 3 6 3 4 3 6 5 4 5 4 6 5 4 6 3 6 5 3 4 5 4 5 4
PC030	2-6	linear shift	2 3 5 2 6 2 4 3 6 5 2 4 4 5 5 2 6 4 5 3 2 6 6 2 4 6
PC031	3-5	linear shift	3 3 4 5 5 3 3 3 5 3 3 4 4 5 5 3 5 3 5 3 3 5 4 3 5 5
PC032	3-5	linear shift	5 4 5 4 5 5 5 5 5 5 3 5 5 5 5 5 5 4 5 4 5 5 5 4 4 5
PC201	1-7	discrete remapping	1 1 7 1 7 1 7 1 7 7 1 7 1 7 7 1 7 1 7 1 1 7 7 1 1 7
PC202	3-5	linear shift	4 3 5 5 4 5 5 5 5 5 4 4 3 5 5 4 5 3 4 3 4 5 4 4 4 5
PC203	1-5	none	4 4 1 2 3 4 1 5 5 1 4 4 3 4 1 4 4 4 4 4 4 3 4 3 4 3
PC204	2-6	linear shift	5 4 6 3 4 5 6 5 6 6 4 5 3 6 5 4 6 3 4 2 6 6 5 2 2 5
PC207	1-7	discrete remapping	4 2 6 1 7 3 7 3 4 5 2 6 1 6 6 3 6 2 6 4 3 6 6 4 5 5
PC208	2-6	linear shift	2 3 6 3 6 3 5 3 5 6 3 5 2 5 6 2 6 6 5 4 4 5 5 5 4 5
PC209	1-7	discrete remapping	1 1 7 1 7 1 7 1 6 7 1 7 1 7 7 1 7 1 7 2 1 7 7 2 1 7
PC210	4-5	linear shift	4 5 4 4 4 4 5 4 4 4 4 5 4 5 5 5 4 5 5 5 4 5 4 4 5 5
PC211	2-6	linear shift	6 6 4 6 3 6 5 6 5 5 6 2 5 5 5 6 4 5 2 5 6 3 2 5 4 3
PC212	1-6	discrete remapping	2 6 5 1 6 4 5 5 6 6 2 6 2 5 6 4 5 2 6 3 2 4 4 3 2 5
PC213	1-7	discrete remapping	1 2 5 4 6 6 4 3 7 6 2 2 2 5 6 2 5 3 4 3 3 6 5 1 3 6
PC214	1-7	discrete remapping	4 2 6 4 7 5 6 4 6 6 3 7 1 7 6 1 6 2 7 1 2 4 6 1 1 7
PC215	2-6	linear shift	5 5 3 5 5 5 2 5 5 3 5 3 5 5 4 5 3 6 4 4 5 5 3 2 5 5
PC216	2-6	linear shift	3 3 6 3 6 5 3 5 5 5 2 5 2 6 5 4 4 2 4 2 3 5 4 2 5 4
PC217	2-6	linear shift	3 3 6 2 6 2 6 3 6 6 2 6 2 6 6 2 6 3 6 2 2 6 5 2 2 6
PC219	2-6	linear shift	3 2 3 2 4 4 5 4 4 4 5 5 3 5 6 3 5 3 4 4 4 5 5 3 3 5
PC221	3-5	linear shift	3 4 5 4 5 4 5 4 5 5 4 5 4 5 5 3 4 4 5 4 4 5 5 4 4 5
PC222	3-5	linear shift	5 4 5 3 4 4 5 5 5 5 4 4 3 5 5 3 4 3 4 3 5 5 4 3 3 4
PC223	2-5	linear shift	3 3 4 2 5 3 4 5 5 4 4 4 3 5 3 3 5 3 5 4 4 5 5 3 4 4
PC224	3-6	linear shift	4 4 6 4 4 4 5 4 4 5 4 3 4 4 5 4 4 3 3 4 4 4 3 3 4 3
PC226	2-6	linear shift	3 2 5 5 6 5 4 3 6 5 4 5 5 6 2 4 5 4 5 2 2 5 4 3 4 5
PC227	1-7	discrete remapping	1 2 6 2 6 3 4 2 7 5 2 6 2 6 6 3 6 2 6 2 2 5 6 3 2 6
PC229	2-6	linear shift	2 2 4 2 6 2 5 2 6 5 2 6 2 6 5 2 6 3 6 3 2 6 6 2 2 6
PC230	2-6	linear shift	2 3 5 2 5 2 4 2 5 3 3 6 2 6 6 3 6 2 6 3 3 4 5 3 2 4
PC231	2-6	linear shift	6 5 4 3 6 6 2 4 4 2 5 5 2 4 4 6 4 2 6 5 2 4 3 4 3 4
PC233	3-6	linear shift	4 3 4 4 5 4 5 4 6 4 4 5 5 6 5 4 5 4 5 3 4 4 5 3 4 4
