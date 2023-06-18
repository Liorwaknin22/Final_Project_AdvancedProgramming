# SISE2601 Project data description
================
Team 18

This Markdown file describes the data folder structure and organization ...

A detailed explanation of the data columns:

*term_id* - Scientific term identifier sampled from Google (37 terms)

*langs* - The language in which the scientific term is sampled (13 languages)

*country* - The country from which the sample was taken (16 countres)

*term* - The scientific term sampled from Google (402 terms)

*type* - The categories of the terms, there are 4 categories according to which the scientific terms are divided and they are:
    1. "Conspiracy Theories" - terms that present conspiracies such as: the earth is flat and more...
    2. "Canonical Scientific Issues" - canonical scientific terms
    3. "Novel Science and Technology Issues" - new issues in science and technology
    4. "Socio-Scientific Issues" - connection between science and society

*code_lang* - Language code

*hl* - The search language entered into Google

*gl* - The interface entered into Google

*Collection_date* - On what date was the sample taken

*Result_number* - In which location was the link to the sampled site (1-19)

*Link* - URL link to the site from which the sample was taken

*coding_completion_date* - Coding completion date 

*correctness_link* - Four categories that characterize the link: 
    1 - The link is correct
    2 - The link is not available
    3 - The link is in a different language than the search
    4 - The link is scientifically irrelevant


*Site_type* - The type of site sampled, divided into 6 categories:
    1 - A site containing text
    2 - A site that contains data in a database
    3 - A site containing videos
    4 - A website containing simulations and illustrations
    5 - A site containing a combination of text and videos and additional simulations
    6 - Other

*content_producer* - Responsible for the production of the scientific content that appears on the site, divided into 17 categories:
    1 - Political bodies (e.g. ministry of health, CDC, FDA, NASA)
    2 - Non-political bodies
    3 - Research organizations (e.g. CERN)
    4 - International organizations (WHO, UN, UNESCO)
    5 - Higher education/academic institution (e.g. university \college)
    6 - Website for official education\ education system
    7 - Informal scientific education and popular science (e.g. science museum, Scientific American)
    8 - Scientific journals or GOOGLE SCHOLAR
    9 - Medical website (e.g. health insurance provider, hospital)
    10 - Encyclopedia or dictionary (e.g. Wikipedia, Oxford dictionary)
    11 - Media and communication (e.g. news sites)
    12 - Commercial / economic (e.g. pharmaceutical companies)
    13 - Satire site
    14 - Social media site (e.g. Twitter, Facebook, LinkedIn etc.)
    15 - Fact checking website
    16 - Blogs
    17 - Other

*recent_information* - Content recency, divided into 4 categories:
    1 - Not mentioned
    2 - Over 10 years
    3 - 5 to 10 years
    4 - Rather new (1 to 5 years)"

*prop_recent_information* - Current proportions of the content, calculated by dividing the previous column by 4.

*author_background* - The author's background, if relevant, divided into 3 categories:
    1- The Author is not mentioned
    2- The author is mentioned but there is no information about their background, or their background is not relevant
    3- The author has relevant expertise to the content

*prop_author_background* - A proportion of the author's background, if applicable, Calculated by dividing the previous column by 3.

*major_scientific_errors*

*prop_major_scientific_errors* - Proportion of whether there are scientific errors is, calculated by dividing the previous column by 2.

*accuracy_scientific_content*

*prop_accuracy_scientific_content* - Proportion of scientific accuracy level, calculated by dividing the previous column by 3

*high_scientific_lang* - Are there any scientific terms that the tagging people do not understand, divided into 3 possibilities:
    1 - Yes
    2 - No
    3 - Not relevant

*explanations_scientific_terms* -
A column that checks whether there are explanations for the incomprehensible scientific terms or whether there is no reference to them:
    1 - Yes
    2 - No

*Jargon_score* - an elaborate calculation of the two previous columns and its purpose is to summarize the level of scientific jargon, there are 3 options:
    1 - There is jargon without an explanation
    2 - There is jargon but it has an explanation
    3 - There is no jargon
    
*prop_Jargon_score*  - Proportion of jargon, calculated by dividing the previous column by 3 (1 - no jargon).

*required_scientific_background* - Is a scientific background required to understand the information on the website, divided into 2 possibilities:
    1 - Yes
    2 - No

*prop_required_scientific_background* - Proportion of whether a scientific background is required, calculated by dividing the previous column by 2.

*sources_available* - a column of the list of all the sources that the model had to mark what the site contained:
    1 - None of the below - none of the categories below
    2 - Others - another
    3 - Place to leave comments\ ask questions - a place on the site where you can comment or ask a question
    4 - Graphs - including graphs
    5 - Relevant multimedia (e.g. video, animation etc.) - contains relevant videos and simulations
    6 - Hyper-links - the website contains hyperlinks to other topics
    7 - Numerical data - contains numerical data
    8 - List of sources - contains a list of relevant sources of information
    9 - Citation or references to relevant literature - Citation or references to relevant literature

*Quality_component_score* - The quality component score is calculated as follows: numerical information + list of sources + citation or reference

*prop_Quality_component_score* - Proportion of the quality component score, calculated by dividing the previous column by 3.

*Accessibility_component_score* -The accessibility component score is calculated as follows: place to leave comments + graphs + relevant multimedia + links.

*prop_Accessibility_component_score* - Proportion of the accessibility component, calculated by dividing the previous column by 4.

*prop_Quality_mean* - The calculation of the average quality component score consists of 5 columns that are considered the quality indicators of the data and they are:
    - prop_recent_information
    - prop_author_background
    - prop_major_scientific_errors
    - prop_accuracy_scientific_content
    - prop_Quality_component_score


*prop_Accessibility_mean* - The calculation of the average accessibility component score consists of 3 columns that are considered the accessibility indicators of the data and they are:
    - prop_Jargon_score
    - prop_required_scientific_background
    - prop_Accessibility_component_score

*reject_or_reinforce_conspiracy_theory* -
Divided into 4 options:
    3 - The content rejects the conspiracy
    2 - Not sure
    1 - The content reinforce the conspiracy
    0 - Irrelevant

*prop_reject_or_reinforce_conspiracy_theory* - Proportion of whether the content repels or reinforces, calculated by dividing the previous column by 3 (1 - this is not conspiratorial).

*malicious_meaning* - Divided into 4 options:
    3 - No
    2 - Not sure
    1 - Yes
    0 - Irrelevant

*prop_malicious_meaning* - The proportion calculated by dividing the previous column by 3 (1 - this is not conspiratorial).

*claims_contradict_accepted_scientific_explanations* - Divided into 4 options:
    3 - No
    2 - Not sure
    1 - Yes
    0 - Irrelevant

*prop_claims_contradict_accepted_scientific_explanations* - The proportion calculated by dividing the previous column by 3 (1 - this is not conspiratorial).

*specific_groups_presented_as_enemy* - Divided into 4 options:
    3 - No
    2 - Not sure
    1 - Yes
    0 - Irrelevant

*prop_specific_groups_presented_as_enemy* - The proportion calculated by dividing the previous column by 3 (1 - this is not conspiratorial).

*prop_Conspiratorial_mean* - The calculation of the average conspiratorial mean score consists of 4 columns and they are:
    - prop_reject_or_reinforce_conspiracy_theory
    - prop_malicious_meaning
    - prop_claims_contradict_accepted_scientific_explanations
    - prop_specific_groups_presented_as_enemy

*daily_reference*

*prop_daily_reference* - The proportion calculated by dividing the previous column by 2.

*local_examples*

*prop_local_examples* - The proportion calculated by dividing the previous column by 2.

*advantages_and_disadvantages_or_risks_and_benefits*

*prop_advantages_and_disadvantages_or_risks_and_benefits* - The proportion calculated by dividing the previous column by 2.

*prop_SSI_mean* - The calculation of the average score for social-scientific issues consists of 4 columns and they are:
    - prop_daily_reference
    - prop_local_examples
    - prop_advantages_and_disadvantages_or_risks_and_benefits