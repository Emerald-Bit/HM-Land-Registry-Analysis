# Analysis of Overseas-Owned Property Acquisition Data and Sanctions Matching

**Business Context and Objective**

Essentially, the business question behind the work was straightforward: could ownership records be linked to sanctions records well enough to support further investigation into patterns of acquisition and possible post-designation ownership changes? In practice, however, that question quickly became a rigorous data-quality and matching problem. It should be noted that property ownership datasets and sanctions lists do not always share a stable universal identifier. Furthermore, name fields are frequently inconsistent, incomplete, and formatted differently across various sources.

To resolve this, I worked primarily in SQL, utilising cleaned Land Registry ownership data alongside a cleaned sanctions list and a sanctions-to-company reference table. The overall workflow combined regex-based standardisation, joins, window functions, and similarity scoring. Ultimately, once the core SQL outputs were successfully in place, Python was used to visualise the main time-series and jurisdiction patterns.

**Stack:** SQL and Snowflake.

**Data Sources:**
•	 UK Sanctions List 
•	 OCOD (Overseas Companies Ownership of Data) 
•	 Companies House PSC Data 

Please view the report for more information.
