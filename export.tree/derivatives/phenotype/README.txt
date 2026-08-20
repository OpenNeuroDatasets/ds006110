Raw behavioural data includes:
  - one TSV file for each questionnaire, accompanied by:
  - one JSON file for each questionnaire, indicating the text prompt for each item

Processed (scored) behavioural data includes:
  - a folder for each session, containing:
    - one TSV file containing scores for each scale, accompanied by:
    - one JSON file for each scale, indicating which items were aggregated to score each subscale, and which operations were performed (e.g. sum, average, etc.)
    - one JSON file indicating the text prompts for all items across all questionnaires. These are also available in the raw data folder but are copied here for convenience. 

Processed (scored) and imputed behavioural data includes:
  - the same folders and file types described above for the non-imputed data
  - for each subscale, data was imputed only when <50% items were missing

Note:
  - "nd" means that data was not disclosed because it was flagged as potentially sensitive (e.g. responses to open questions, reflections, or demographic information)