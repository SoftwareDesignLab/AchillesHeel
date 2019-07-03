# AchillesHeel
This repository thas the data for the paper "Achilles' Heel of Plug-and-Play Software Architectures: A Grounded Theory Based Approach"(ESEC/FSE 2019).



## Folder Structure

- **AllRetrievedData**: This folder contains all the CVEs that were retrieved from the National Vulnerability Database (Section 2.2.2). These vulnerability reports are released as CSV files containing:
  - cve_id (vulnerability identifier)
  - description (description of the security issue)
  - published_date (the date the CVE was published at NVD)
  - references (list of URLs to external Websites that may contain more details about the CVE)
- **FilteredCVEs**: This folder contains the output of our three complementary filtering approach (Section 2.2.3). The output for each project is an Excel Sheet that contains:
  - cve_id (vulnerability identifier)
  - keyword-based (This column has an “X” if the CVE matched the heuristic of the keyword-based approach. Otherwise, it has a N/A)
  - component-based (This column has an “X” if the CVE matched the heuristic of the component-based approach. Otherwise, it has a N/A)
  - file-based (This column has an “X” if the CVE matched the heuristic of the file-based approach. Otherwise, it has a N/A)
- **CVESummaries**: It contains the Excel Sheets with the CVE summaries (context, problem, solution) as well as the augmenting links (commit url, and issue tracking system URL) that we manually collected (Section 2.2.4).
- **CodedCVEs**: It contains PDF with open codes for each project. These PDFs have the analyzed CVEs with highlights of the keypoints as well as their corresponding codes. There is also an Excel Sheet with the frequencies of each code per software project as well as a chart depicting the frequency of each code.
- **Core Categories Mapped to CVEs**: This folder has the list of CVEs per core category (i.e, type of plug-and-play vulnerability). 
- **Memos**: It contains the notes taken throughout the data analysis ("memoing"). 
