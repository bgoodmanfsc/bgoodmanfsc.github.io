# CTDN Data Model

The following model is being proposed for usage in the Pilot version of the Clinical Trial Distribution Network.  We are open to all contributions or suggested edits to this data model. 

| Entity                                           | Data Type             | Attribute                                      | Parameters | Example |
| ------------------------------------------------ | --------------------- | ---------------------------------------------- | ---------- | ------- |
| NCT Number                                       | Trial                 | Numeric                                        |            |         |
| CT Name - Official Research Title                | Trial                 | String                                         |            |         |
| CT Description - Brief Description of Research   | Trial                 | String                                         |            |         |
| Age - Required Age of the Patient                | Inclusion / Exclusion | Min, Max - 18 years threshold                  | 1 to 120   |         |
| Stage - Stage of Disease                         | Inclusion / Exclusion | +, <, >, !, Null - Stage 4 Exclusion           |            |         |
|                                                  |                       | Stage 1, Stage 2, Stage 3, Stage 4             |            |         |
| Biomarker Status - Select Biomarker              | Inclusion / Exclusion | True, False, Either / OR                       |            |         |
| Gender - Required Gender of the Patient          | Inclusion             | Male, Female, Either, Unidentified             |            |         |
| Phase - Phase of the Clinical Trial              | Trial                 | Phase 1, Phase 2, Phase 3                      |            |         |
| Origin Company - Primary Sponsor of the Research | Trial                 | String                                         |            |         |
| Recruitment Status - Still recruiting or not     | Trial                 | True - False, Deadline Date                    |            |         |
| Location                                         | Trial                 | Address, Zip Code, Country                     |            |         |
| Cancer Type                                      | Inclusion / Exclusion | Cancer Types, MM Types, Other                  |            |         |
| Cancer SubType                                   | Inclusion / Exclusion | Cancer Sub Types, MM Sub Types, Other          |            |         |
| Presence of Metastases                           | Inclusion / Exclusion | True, False                                    |            |         |
| Treatments                                       | Inclusion             | No Prior Treatments                            |            |         |
| Treatments                                       | Exclusion             | chemotherapy, immunotherapy, hormonal therapy, |            |         |
|                                                  |                       | radiation, or investigational therapy          |            |         |
| Performance Status                               | Inclusion             | ECOG performance status of 0 or 1              |            |         |
| Performance Status                               | Exclusion             |                                                |            |         |
|                                                  |                       |                                                |            |         |
| Plain Language Summary                           |                       |                                                |            |         |
| Purpose of the Study                             | Plain Language        | String, Paragraph                              |            |         |
| Who is it for                                    | Plain Language        | String, Paragraph                              |            |         |
| What is involved                                 | Plain Language        | String, Paragraph                              |            |         |
| How can I learn more                             | Plain Language        | String, Paragraph                              |            |         |
| - Resource                                       | Plain Language        | String                                         |            |         |
| - Link                                           | Plain Language        | url                                            |            |         |
| Visits Required per Month                        | Plain Language        | Numeric                                        | 1 - 10     |         |

