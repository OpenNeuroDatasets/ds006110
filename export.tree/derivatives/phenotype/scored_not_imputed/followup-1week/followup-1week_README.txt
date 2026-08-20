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

Total participants processed: 59
Total participants transformed: 56
Discrete remapping participants: 44
Linear shift participants: 12

participant_id	transformation_applied	original_values	recoded_values
PC001	discrete remapping	5 2 6 3 3 7 3 3 3 3 6 3 6 3 3 3 4 3 3 2 2 3 6 2 3 3	4 2 4 2 2 5 2 2 2 2 4 2 4 2 2 2 3 2 2 2 2 2 4 2 2 2
PC002	linear shift	7 7 4 7 4 6 4 7 4 4 7 4 7 4 4 7 4 7 4 6 7 4 3 7 7 4	5 5 2 5 2 4 2 5 2 2 5 2 5 2 2 5 2 5 2 4 5 2 1 5 5 2
PC003	discrete remapping	6 7 5 1 2 7 4 1 5 4 7 3 1 5 5 1 5 1 4 1 1 2 4 1 1 4	4 5 4 1 2 5 3 1 4 3 5 2 1 4 4 1 4 1 3 1 1 2 3 1 1 3
PC004	discrete remapping	3 4 6 6 3 3 7 2 6 6 2 6 3 6 7 4 2 3 3 3 3 1 6 3 2 2	2 3 4 4 2 2 5 2 4 4 2 4 2 4 5 3 2 2 2 2 2 1 4 2 2 2
PC005	discrete remapping	6 6 3 6 3 3 3 6 3 3 7 3 2 2 3 6 3 2 2 2 2 2 2 2 2 2	4 4 2 4 2 2 2 4 2 2 5 2 2 2 2 4 2 2 2 2 2 2 2 2 2 2
PC006	discrete remapping	2 6 4 6 2 3 3 3 3 3 6 2 6 4 3 6 4 7 3 6 6 3 3 7 6 4	2 4 3 4 2 2 2 2 2 2 4 2 4 3 2 4 3 5 2 4 4 2 2 5 4 3
PC007	linear shift	2 3 2 3 2 3 2 2 2 2 6 6 6 2 2 3 2 6 2 3 2 6 2 2 3 3	1 2 1 2 1 2 1 1 1 1 5 5 5 1 1 2 1 5 1 2 1 5 1 1 2 2
PC008	linear shift	3 2 4 4 4 4 2 2 4 4 4 2 2 3 4 3 3 2 2 3 3 4 3 4 4 2	3 1 5 5 5 5 1 1 5 5 5 1 1 3 5 3 3 1 1 3 3 5 3 5 5 1
PC009	discrete remapping	1 1 3 1 2 1 2 1 2 3 1 7 1 3 3 1 3 7 2 7 2 3 3 7 1 3	1 1 2 1 2 1 2 1 2 2 1 5 1 2 2 1 2 5 2 5 2 2 2 5 1 2
PC010	discrete remapping	6 7 3 7 3 7 3 6 4 4 7 3 7 4 4 6 4 7 3 6 3 4 3 6 2 3	4 5 2 5 2 5 2 4 3 3 5 2 5 3 3 4 3 5 2 4 2 3 2 4 2 2
PC011	discrete remapping	3 3 2 3 2 6 6 6 2 6 3 6 3 2 7 3 2 3 6 3 2 7 3 7 2 6	2 2 2 2 2 4 4 4 2 4 2 4 2 2 5 2 2 2 4 2 2 5 2 5 2 4
PC012	discrete remapping	1 1 1 1 4 1 2 6 5 4 7 4 7 5 4 7 4 7 4 1 2 4 4 1 6 4	1 1 1 1 3 1 2 4 4 3 5 3 5 4 3 5 3 5 3 1 2 3 3 1 4 3
PC013	discrete remapping	2 1 3 2 5 2 4 7 5 7 1 4 1 4 4 1 2 1 5 1 1 4 4 1 6 3	2 1 2 2 4 2 3 5 4 5 1 3 1 3 3 1 2 1 4 1 1 3 3 1 4 2
PC014	discrete remapping	7 6 3 2 3 6 3 6 3 3 7 2 6 3 3 6 3 6 2 3 2 3 3 6 3 3	5 4 2 2 2 4 2 4 2 2 5 2 4 2 2 4 2 4 2 2 2 2 2 4 2 2
PC015	discrete remapping	7 3 2 7 4 2 7 2 4 2 7 3 7 2 2 2 3 7 3 6 7 2 3 2 7 3	5 2 2 5 3 2 5 2 3 2 5 2 5 2 2 2 2 5 2 4 5 2 2 2 5 2
PC016	discrete remapping	6 7 7 7 6 6 7 6 2 6 2 7 3 7 6 2 6 4 2 2 2 2 2 3 3 2	4 5 5 5 4 4 5 4 2 4 2 5 2 5 4 2 4 3 2 2 2 2 2 2 2 2
PC017	discrete remapping	6 6 2 7 2 6 2 6 3 3 6 2 6 3 3 6 3 6 2 6 6 2 2 7 6 2	4 4 2 5 2 4 2 4 2 2 4 2 4 2 2 4 2 4 2 4 4 2 2 5 4 2
PC018	discrete remapping	6 6 3 2 3 3 2 2 2 2 6 2 6 2 3 6 2 7 2 6 6 2 2 7 2 2	4 4 2 2 2 2 2 2 2 2 4 2 4 2 2 4 2 5 2 4 4 2 2 5 2 2
PC019	discrete remapping	6 2 3 6 2 3 4 2 6 2 6 6 7 3 3 6 6 6 2 3 2 6 3 7 3 3	4 2 2 4 2 2 3 2 4 2 4 4 5 2 2 4 4 4 2 2 2 4 2 5 2 2
PC020	none	1 1 5 1 1 1 5 1 5 5 1 5 1 5 5 1 5 1 5 1 1 5 5 1 1 5	1 1 5 1 1 1 5 1 5 5 1 5 1 5 5 1 5 1 5 1 1 5 5 1 1 5
PC022	linear shift	3 2 3 2 2 2 3 3 6 3 6 2 2 2 3 3 2 6 2 3 2 6 2 3 6 2	2 1 2 1 1 1 2 2 5 2 5 1 1 1 2 2 1 5 1 2 1 5 1 2 5 1
PC023	discrete remapping	6 6 3 7 3 2 3 3 3 3 6 3 6 4 3 6 3 6 3 6 6 4 4 6 6 3	4 4 2 5 2 2 2 2 2 2 4 2 4 3 2 4 2 4 2 4 4 3 3 4 4 2
PC025	linear shift	2 6 2 3 3 3 6 2 3 6 4 2 6 4 2 3 3 3 3 6 2 6 2 2 6 6	1 5 1 2 2 2 5 1 2 5 3 1 5 3 1 2 2 2 2 5 1 5 1 1 5 5
PC026	discrete remapping	1 7 4 7 4 7 4 1 4 4 1 5 3 5 5 7 4 2 4 3 6 4 3 7 3 5	1 5 3 5 3 5 3 1 3 3 1 4 2 4 4 5 3 2 3 2 4 3 2 5 2 4
PC027	discrete remapping	6 7 4 7 3 6 4 6 3 4 6 3 7 4 4 7 3 7 3 6 3 3 3 7 2 3	4 5 3 5 2 4 3 4 2 3 4 2 5 3 3 5 2 5 2 4 2 2 2 5 2 2
PC028	discrete remapping	2 2 2 7 6 2 7 3 2 6 6 2 2 6 3 2 2 6 2 4 2 6 2 3 3 2	2 2 2 5 4 2 5 2 2 4 4 2 2 4 2 2 2 4 2 3 2 4 2 2 2 2
PC029	discrete remapping	2 2 5 6 5 2 3 7 4 5 2 3 2 5 5 3 5 3 4 2 7 5 4 7 4 4	2 2 4 4 4 2 2 5 3 4 2 2 2 4 4 2 4 2 3 2 5 4 3 5 3 3
PC030	discrete remapping	6 6 3 7 4 7 3 6 3 3 7 3 2 4 3 6 3 2 3 7 7 3 3 7 7 4	4 4 2 5 3 5 2 4 2 2 5 2 2 3 2 4 2 2 2 5 5 2 2 5 5 3
PC031	linear shift	2 2 6 3 2 2 6 2 3 6 2 2 6 3 6 2 3 6 2 6 3 3 2 2 3 2	1 1 5 2 1 1 5 1 2 5 1 1 5 2 5 1 2 5 1 5 2 2 1 1 2 1
PC032	linear shift	3 3 3 2 3 3 3 3 3 3 2 3 6 4 3 2 3 6 2 6 3 3 2 6 3 2	2 2 2 1 2 2 2 2 2 2 1 2 5 3 2 1 2 5 1 5 2 2 1 5 2 1
PC201	none	1 1 5 1 5 1 4 1 5 5 1 5 1 5 5 1 5 1 5 1 1 5 1 1 1 5	1 1 5 1 5 1 4 1 5 5 1 5 1 5 5 1 5 1 5 1 1 5 1 1 1 5
PC202	linear shift	2 2 3 3 3 2 3 2 3 3 2 2 6 3 3 2 2 6 2 2 2 3 3 3 2 3	1 1 2 2 2 1 2 1 2 2 1 1 5 2 2 1 1 5 1 1 1 2 2 2 1 2
PC203	discrete remapping	7 6 7 7 6 7 1 6 6 1 2 6 7 6 6 6 2 1 3 6 2 3 2 7 7 7	5 4 5 5 4 5 1 4 4 1 2 4 5 4 4 4 2 1 2 4 2 2 2 5 5 5
PC204	discrete remapping	3 6 3 3 3 6 4 2 4 4 6 3 6 5 4 3 5 6 3 1 3 4 2 7 2 3	2 4 2 2 2 4 3 2 3 3 4 2 4 4 3 2 4 4 2 1 2 3 2 5 2 2
PC205	discrete remapping	7 6 3 1 2 7 7 7 4 7 7 3 6 3 3 7 3 6 3 7 4 7 4 2 3 4	5 4 2 1 2 5 5 5 3 5 5 2 4 2 2 5 2 4 2 5 3 5 3 2 2 3
PC207	discrete remapping	6 6 4 6 4 2 4 2 2 6 6 3 6 3 4 6 4 7 2 2 6 4 4 6 3 3	4 4 3 4 3 2 3 2 2 4 4 2 4 2 3 4 3 5 2 2 4 3 3 4 2 2
PC208	discrete remapping	7 2 4 6 3 6 4 6 3 4 3 3 6 4 4 6 5 6 3 3 2 6 3 4 2 3	5 2 3 4 2 4 3 4 2 3 2 2 4 3 3 4 4 4 2 2 2 4 2 3 2 2
PC209	discrete remapping	1 1 4 1 5 7 5 1 4 5 5 5 1 5 5 1 5 1 5 7 1 5 5 7 7 5	1 1 3 1 4 5 4 1 3 4 4 4 1 4 4 1 4 1 4 5 1 4 4 5 5 4
PC210	linear shift	2 2 3 2 3 2 3 3 3 3 3 2 3 3 2 2 2 3 3 3 2 2 2 3 3 4	1 1 3 1 3 1 3 3 3 3 3 1 3 3 1 1 1 3 3 3 1 1 1 3 3 5
PC211	discrete remapping	4 4 6 3 6 3 6 4 3 3 3 7 6 2 4 4 3 2 6 2 4 3 2 2 4 6	3 3 4 2 4 2 4 3 2 2 2 5 4 2 3 3 2 2 4 2 3 2 2 2 3 4
PC212	discrete remapping	6 4 3 2 4 3 3 2 2 3 7 4 2 2 4 6 3 6 4 3 2 2 3 3 3 4	4 3 2 2 3 2 2 2 2 2 5 3 2 2 3 4 2 4 3 2 2 2 2 2 2 3
PC213	discrete remapping	6 3 6 3 2 3 6 6 4 2 2 6 3 4 3 6 4 2 2 1 3 6 6 1 2 6	4 2 4 2 2 2 4 4 3 2 2 4 2 3 2 4 3 2 2 1 2 4 4 1 2 4
PC214	discrete remapping	6 6 4 3 4 1 4 2 5 3 1 2 1 3 3 7 3 1 4 1 1 3 4 7 7 4	4 4 3 2 3 1 3 2 4 2 1 2 1 2 2 5 2 1 3 1 1 2 3 5 5 3
PC215	discrete remapping	4 3 2 4 2 3 6 3 4 6 3 6 3 3 3 3 3 3 2 3 3 3 7 6 3 2	3 2 2 3 2 2 4 2 3 4 2 4 2 2 2 2 2 2 2 2 2 2 5 4 2 2
PC216	discrete remapping	6 1 4 7 4 1 3 7 4 4 7 2 7 4 4 6 2 6 3 4 7 3 3 1 1 3	4 1 3 5 3 1 2 5 3 3 5 2 5 3 3 4 2 4 2 3 5 2 2 1 1 2
PC217	discrete remapping	7 7 4 7 5 7 5 7 3 5 6 4 1 4 5 7 5 1 4 1 1 5 4 1 1 5	5 5 3 5 4 5 4 5 2 4 4 3 1 3 4 5 4 1 3 1 1 4 3 1 1 4
PC218	linear shift	2 3 6 3 6 3 2 3 6 2 3 6 2 2 3 4 6 2 6 3 2 6 6 3 3 6	1 2 5 2 5 2 1 2 5 1 2 5 1 1 2 3 5 1 5 2 1 5 5 2 2 5
PC219	discrete remapping	2 6 3 7 2 7 2 2 6 2 2 2 7 6 2 6 6 7 6 6 7 6 6 6 6 6	2 4 2 5 2 5 2 2 4 2 2 2 5 4 2 4 4 5 4 4 5 4 4 4 4 4
PC221	linear shift	6 2 2 6 3 6 2 2 2 2 6 3 6 2 2 6 3 6 3 2 6 2 3 6 6 2	5 1 1 5 2 5 1 1 1 1 5 2 5 1 1 5 2 5 2 1 5 1 2 5 5 1
PC222	discrete remapping	3 2 6 6 2 2 6 3 4 6 2 6 6 3 6 2 3 6 6 6 3 3 3 7 6 2	2 2 4 4 2 2 4 2 3 4 2 4 4 2 4 2 2 4 4 4 2 2 2 5 4 2
PC223	discrete remapping	2 2 6 3 3 7 3 3 2 3 6 2 3 3 2 4 3 6 2 2 2 3 6 2 3 2	2 2 4 2 2 5 2 2 2 2 4 2 2 2 2 3 2 4 2 2 2 2 4 2 2 2
PC224	linear shift	2 2 4 2 2 3 4 3 2 3 2 2 2 3 3 2 3 2 2 2 2 2 2 3 3 2	1 1 5 1 1 3 5 3 1 3 1 1 1 3 3 1 3 1 1 1 1 1 1 3 3 1
PC226	discrete remapping	6 7 3 7 4 6 6 7 4 7 7 4 2 4 6 7 4 3 3 7 7 4 2 7 6 3	4 5 2 5 3 4 4 5 3 5 5 3 2 3 4 5 3 2 2 5 5 3 2 5 4 2
PC227	discrete remapping	7 6 4 2 4 6 3 6 3 4 7 4 6 3 5 7 3 6 4 6 3 2 3 6 2 3	5 4 3 2 3 4 2 4 2 3 5 3 4 2 4 5 2 4 3 4 2 2 2 4 2 2
PC229	discrete remapping	7 7 2 7 4 7 4 7 4 4 7 4 7 4 4 7 4 7 4 7 6 4 4 7 7 4	5 5 2 5 3 5 3 5 3 3 5 3 5 3 3 5 3 5 3 5 4 3 3 5 5 3
PC230	discrete remapping	1 7 4 1 4 1 6 7 3 3 7 4 7 4 5 7 5 7 4 6 7 3 7 2 7 4	1 5 3 1 3 1 4 5 2 2 5 3 5 3 4 5 4 5 3 4 5 2 5 2 5 3
PC231	discrete remapping	4 3 2 3 4 4 6 2 2 2 2 3 6 3 3 2 2 7 3 3 7 2 2 3 2 2	3 2 2 2 3 3 4 2 2 2 2 2 4 2 2 2 2 5 2 2 5 2 2 2 2 2
PC233	discrete remapping	7 7 4 7 4 6 3 6 3 4 2 3 2 4 3 6 3 2 3 6 6 2 3 6 2 2	5 5 3 5 3 4 2 4 2 3 2 2 2 3 2 4 2 2 2 4 4 2 2 4 2 2

Emotional Breakthrough Inventory (EBI)
- Modified prompt from "How much are the following statements true of your experience"
- Changed to "How much are the following statements true of your (psilocybin) experience"

Life Changes Inventory – Revised (LCI-R)
- Added specific instructions framing each statement to begin with "Since my psilocybin experience..."
- Provided clear rating scale description:
  a) Strongly increased (SI)
  b) Increased somewhat (I)
  c) Not changed (NC)
  d) Decreased somewhat (D)
  e) Strongly decreased (SD)