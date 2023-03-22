## CTDN Data Model

The following model is being proposed for usage in the Pilot version of the Clinical Trial Distribution Network. We are open to all contributions or suggested edits to this data model.

| Entity                                           | Data Category         | Data Type         | Parameters                        | Example                                                                         |
|-------------|-------------|-------------|-------------|-----------------------|
| NCT Number                                       | Trial                 | String            | None                              | "NCT01980823"                                                                   |
| CT Name - Official Research Title                | Trial                 | String            | None                              | "Metformin & Atorvastatin Before Surgery to Study Their Effect on Cancer Cells" |
| CT Description - Brief Description of Research   | Trial                 | String            | None                              |                                                                                 |
| Age - Required Age of the Patient                | Inclusion / Exclusion | Integer           | 1 to 120                          | 45                                                                              |
| Stage - Stage of Disease                         | Inclusion / Exclusion | Array             | Stage 1 to Stage 4                | Stage 2                                                                         |
| Biomarker Status - Select Biomarker              | Inclusion / Exclusion | Boolean           | TBD                               | HER2                                                                            |
| Gender - Required Gender of the Patient          | Inclusion / Exclusion | Boolean           | Male, Female                      | Male                                                                            |
| Phase - Phase of the Clinical Trial              | Trial                 | Array             | Phase 1, Phase 2, Phase 3         | Phase 2                                                                         |
| Origin Company - Primary Sponsor of the Research | Trial                 | String            | None                              | Roche                                                                           |
| Recruitment Status - Still recruiting or not     | Trial                 | Boolean           | Recruiting, Not Recruiting        | Recruiting                                                                      |
| Location                                         | Trial                 | String            | To be divided into subtypes       | Jean Francois Leemans 34, Auderghem Brussels 1160                               |
| Cancer Type                                      | Inclusion / Exclusion | Array             | Cancer Types - Per Indication     | Breast Cancer                                                                   |
| Cancer SubType                                   | Inclusion / Exclusion | Array             | Cancer Sub Types - Per Indication |                                                                                 |
| Presence of Metastases                           | Inclusion / Exclusion | Boolean           | True, False                       | False                                                                           |
| Treatments                                       | Inclusion             | Boolean           | True, False                       |                                                                                 |
| Treatments                                       | Exclusion             | Array             | TBD per Indication                | Chemotherapy, Immunotherapy, Hormonal Therapy,                                  |
| Performance Status                               | Inclusion             | Boolean           | ECOG performance status of 0 or 1 | ECOG performance status of 0                                                    |
| Performance Status                               | Exclusion             |                   |                                   |                                                                                 |
|                                                  |                       |                   |                                   |                                                                                 |
| Plain Language Summary                           |                       |                   |                                   |                                                                                 |
| Purpose of the Study                             | Plain Language        | String, Paragraph |                                   |                                                                                 |
| Who is it for                                    | Plain Language        | String, Paragraph |                                   |                                                                                 |
| What is involved                                 | Plain Language        | String, Paragraph |                                   |                                                                                 |
| How can I learn more                             | Plain Language        | String, Paragraph |                                   |                                                                                 |
| \- Resource                                      | Plain Language        | String            |                                   |                                                                                 |
| \- Link                                          | Plain Language        | url               |                                   |                                                                                 |
| Visits Required per Month                        | Plain Language        | Numeric           | 1 - 10                            |                                                                                 |
