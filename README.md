# Managing Knowledge in the Context of ITIL

Knowledge Management (KM) became an integral part of ITIL v3 during the Service Transition phase, which focuses on the development and implementation of new or modified services. Before ITIL v3, the management of knowledge fell under the purview of the Incident and Problem Management processes. However, with the introduction of a dedicated Knowledge Management process, ITIL v3 now offers comprehensive guidelines and **workflows** for effectively managing all knowledge throughout the **Service Management life cycle**. Additionally, ITIL v3 emphasizes the integration of the Knowledge Management process with Service Desk (Interaction Management), Incident Management, and Problem Management.

**The primary objective of Knowledge Management is to empower your organization to access, update, and share all relevant knowledge related to the Service Management life cycle efficiently**. The benefits of Knowledge Management encompass, among other things:

1.  Improved efficiency in handling knowledge.
2.  Decreased likelihood of multiple stakeholders independently attempting to solve the same problem without sharing knowledge first.
3.  Control over access to sensitive information for specific individuals.

At the core of Knowledge Management lies a repository known as the Service Knowledge Management System (SKMS). A typical SKMS houses all knowledge in a Knowledge Base, with items referred to as Knowledge Documents. These documents can include various attachment types, such as text files and graphics files. The SKMS also **provides tools for crucial tasks like report generation**.

According to Processes and Best Practices, Knowledge Management is the process responsible for supplying knowledge to all other **IT Service Management processes**. Due to the extensive number of processes involved, the document's scope is limited to those processes associated with storing new **KM** documents and updating, archiving, and retiring existing KM documents.


# Knowledge Management Application

The Knowledge Management application in Service Manager assists in overseeing all information associated with Interactions, Incidents, and Problems.
 

### Types of Knowledge Documents in Service Manager
> Document types serve as templates for documents within the Knowledge Management system. Knowledge Management encompasses various default document types:
> 
-   Question/Answer
-   Problem-Solution
-   Reference
-   Error Message/Cause
-   External

#### Knowledge Management Categories
Each document within the knowledge base is categorized into a specific document category. Knowledge document categories are structured hierarchically, with top-level categories and subcategories. Each subcategory has a parent category, which is the category directly above it in the hierarchical list. Similarly, a top-level category serves as the parent category for the immediate subcategory below it in the ordered list of categories.

### Knowledge Groups
Knowledge groups allow you to gather users into specific groups, granting them access to collaborate on a shared set of documents. A knowledge group could represent a department, a collective of document authors, or a specialized group within your organization, such as subject matter experts.

By associating a knowledge group with at least one document category or subcategory, members of that knowledge group gain access to documents within the specified category and all its subcategories. Access privileges vary, ranging from search and view capabilities to publishing privileges, depending on the assigned knowledge profile(s) to the category.


### Knowledge Management Profiles
  
The Knowledge Management profiles govern both access to knowledge documents and rights related to document creation, editing, and administration.

In each security profile, a specific (named) profile is directly linked to the categories and subcategories to which the designated capabilities are applicable. Each security profile corresponds to a document category or subcategory, providing a user with access to documents outlined by the profile-to-category mapping, including all subcategories within that branch of the category tree.

Profiles can be customized to selectively choose certain capabilities, effectively creating sub-profiles. For instance, certain users may be restricted from publishing knowledge documents externally, limiting their privileges to internal publishing.

The pre-configured KM security profiles are succinctly outlined in the following table:
| KM Profile | Privileges |
|--|--|
| DEFAULT | Using this profile, a user has the capability to explore and examine knowledge documents published externally within the categories accessible through this profile. Additionally, they can provide feedback on these documents. |
| INTERNAL USER | Under this profile, a user is able to search and access knowledge documents published externally within the categories permitted by this profile. Similarly, they can search and view knowledge documents that are internally approved, again within the categories accessible through this profile. Additionally, users can provide feedback on these documents. |
| KCS I | Author and contribute knowledge documents. |
| KCS EDITOR | Create and edit knowledge documents authored by the editor in the workflow, specifically within the categories accessible through this profile. |
| KCS II | Create knowledge documents, contribute to knowledge documents, edit published documents without initiating workflow (edit in place), and internally publish documents. Additionally, view adaptive learning data when the adaptive learning feature is activated in the system. |
| KCS III | Create knowledge documents, contribute to knowledge documents, edit published documents without initiating workflow (edit in place), and publish documents both internally and externally. Additionally, access adaptive learning data when the adaptive learning feature is active in the system. |
| KM ADMIN | Create knowledge documents, contribute to knowledge documents, edit published documents directly without initiating workflow (edit in place), and publish documents for both internal and external use. Additionally, access adaptive learning data when the adaptive learning feature is activated in the system. |

## Knowledge Management Process Overview
![enter image description here](https://github.com/QueeNFrisk/KnowledgeManagement/blob/master/contribute_and_approve_km_doc_st7.0.png?raw=true)
### # Knowledge Management User Roles
The following table describes the responsibilities of the Knowledge Management roles.

**Knowledge Management Process Owner**:
-    Accountable for the definition, management, governance and improvement of the KM Process
-   Ensures that the KM process and working practices are effective and efficient
-   Ensures that all stakeholders are sufficiently involved in the KM process
-   Ensures that (business) management is sufficiently informed as to the volume, impact and cost of Knowledge
-   Ensures tight linkage between the KM process and other related processes

**Knowledge Manager**:
-   Implementation and ongoing management of the Knowledge Management process
-   Championing the Knowledge Management process with people at all levels
-   Management of Knowledge Analysts
-   Ensuring process efficiency and consistency
-   Final QA and approval of all Knowledge Submissions
-   Deciding the scope of publishing (external and / or internal)
-   Continual improvement of the Knowledge Library and process
-   Fast tracking urgent 'Hot News' notices through the KM process
-   Reviewing KM reports
-   Identifying, allocating and tracking continual improvement actions and maintenance activities

**Knowledge Expert**
-   Reviewing and amending Knowledge Submissions
-   Rejecting Knowledge Submissions based on technical content
-   Assisting with reviews of Knowledge Documents for currency and relevance

**Knowledge Analyst**
-   Administering the KM process
-   Reviewing Knowledge Candidates for basic content, spelling, format, readability, duplication and editing to achieve a consistent quality level
-   Rejecting inappropriate or duplicated Knowledge Submissions
-   Co-ordinating Knowledge Expert reviews and reviewing Knowledge Document feedback and identifying improvements
-   Producing and distributing KM reports
-   Driving periodic reviews of Knowledge and co-ordinating and / or performing improvement actions
-   Retiring Knowledge Documents no longer deemed relevant

**Knowledge Contributor**
-   Identifying Knowledge Submissions
-   Identifying changes required to existing Knowledge Documents
-   Submitting new or revised Knowledge Submissions
-   Assisting with reviews of Knowledge Documents for currency and relevance

### Key performance indicators for Knowledge Management
The Key Performance Indicators (KPIs) presented in the table below serve as valuable tools for assessing your Knowledge Management processes. Periodically graphing KPI data is beneficial for visualizing trend information. It's important to note that while Knowledge Management provides certain data, additional tools may be required to comprehensively report on all your KPI requirements.


**Number of KM documents created**
The overall count of Knowledge Management documents within your organization will increase progressively. Nevertheless, as time passes, older KM documents will naturally become obsolete and should be phased out. Keep track of the number of newly generated documents to assess the ideal growth rate over a specified period.

**Number of times a KM document is accessed**
A valuable document is frequently accessed. Utilize this metric to identify the documents with the highest and lowest levels of usefulness.

**Number of KM documents used to resolve Interactions**
The ultimate goal of KM documents is to contribute to resolutions. Keep track of the quantity of KM documents that result in resolutions for Interactions. This monitoring helps assess the effectiveness of your Service Desk in accessing and reusing knowledge.

**Number of KM documents used to resolve Incidents**
Track the quantity of KM documents contributing to the resolution of Incidents to assess the effectiveness of KM documents in resolving escalated and critical issues.

**Number of KM documents with an expired review date**
To guarantee the effectiveness of the document publishing process, keep an eye on the quantity of documents that haven't undergone timely review.

<br />

### [RACI Matrix For Knowledge Management](https://es.wikipedia.org/wiki/Matriz_de_asignaci%C3%B3n_de_responsabilidades)
A Responsible, Accountable, Consulted, and Informed (RACI) diagram or matrix is employed to delineate the roles and duties of different teams or individuals involved in project delivery or process operation. It proves particularly beneficial in elucidating roles and responsibilities in projects and processes that involve collaboration across functions or departments.


### Contribute and Verify Knowledge Document (Process ST 0.1).
The initiation of the Contribute and Approve Knowledge Document process involves the submission of a KM document. This contribution can take the form of authoring knowledge articles or utilizing external documents that are uploaded into a knowledge base. The authoring process is facilitated through the use of a rich-text editor, and attachments, including images, text files, Word files, or PDFs, can be added.

The process commences with a contributor either creating a new submission or revising an existing knowledge document. The contributor specifies a documentation type, inputs basic details, selects a category type, and submits the draft for review by a Knowledge Analyst. The analyst holds the authority to edit, accept, or reject the document. If deemed necessary, the document may be forwarded to a Knowledge Expert, who also possesses the ability to edit, accept, or reject it. Typically, the Knowledge Expert serves as a subject-matter expert, possessing in-depth understanding of a specific topic and the capability to assess the accuracy and currency of the KM document. The final decision regarding the acceptance or revision of the document lies with the Knowledge Manager. If the document satisfies all KM publication criteria, the Knowledge Manager approves and publishes it. The workflow for Contribute and Approve KM Doc/Change Request is depicted in the accompanying figure.

![enter image description here](https://github.com/QueeNFrisk/KnowledgeManagement/blob/master/contribute_and_approve_km_doc_st7.1.png?raw=true)


| Process ID | Procedure or Decision | Description | Role |
|--|--|--|--|
| ST 0.1.1 | Populate Knowledge details | Input information related to the Knowledge Submission into Service Manager. Recommendations for new or enhanced KM documents can originate from various sources, including Incident and Problem Management. Refer to ST 0.1.2 to choose the relevant Knowledge category. | Knowledge Contributor |
| ST 0.1.2 | Select Knowledge category | Choose the relevant category from the options provided in Service Manager. Proceed to ST 0.1.3 to initiate the submission of the Knowledge Submission. | Knowledge Contributor |
| ST 0.1.3 | Submit for approval | Send the Knowledge Submission for approval from the Knowledge team. Visit ST 0.1.4 for the Knowledge Analyst to conduct an initial review and verify for any duplicates. | Knowledge Contributor |
| ST 0.1.4 | Initial review and duplicates check | Review the Knowledge Submission to verify the presence of all necessary information in the correct format. Additionally, check against other recent Knowledge Submissions to prevent duplicating efforts. Refer to ST 0.1.5 to decide whether to reject the Knowledge Submission. | Knowledge Analyst |
| ST 0.1.5 | Reject Knowledge Submission? | The Knowledge Submission will face rejection if the Knowledge Analyst deems it invalid or a duplicate of an existing proposal. In the affirmative, proceed to ST 0.1.6 to communicate the reasons for rejection to the Knowledge Contributor. In the negative, move to ST 0.1.7 to edit the Knowledge Submission. | Knowledge Analyst |
| ST 0.1.6 | Retire Knowledge Submission and inform Contributor of reason(s) | Notify the Knowledge Contributor about the reasons for rejecting the Knowledge Submission. The 'Contribute and Approve Knowledge' process concludes. | Knowledge Analyst |
| ST 0.1.7 | Edit Knowledge Submission and notify Contributor | Include any comments or supplementary information with the Knowledge Submission in preparation for subsequent review and approval. Inform the Knowledge Contributor. Proceed to ST 0.1.8 to assess whether an expert review is necessary. | Knowledge Analyst |
| ST 0.1.8 | Expert Review Required? | Certain Knowledge Submissions are exclusively handled by the Knowledge team. If the Knowledge Submission pertains to a specialized area, an expert will be invited to review and approve it. If affirmative, proceed to ST 0.1.9 for the Knowledge Expert to assess the Knowledge Submission. If negative, move on to ST 0.1.12 for the Knowledge Manager to conduct a QA review. | Knowledge Analyst |
| ST 0.1.9 | Perform Expert review | Evaluate the Knowledge Submission. Proceed to ST 0.1.10 to decide whether to reject the Knowledge Submission. | Knowledge Expert |
| ST 0.1.10 | Reject Knowledge Submission? | Should the Knowledge Expert deem the Knowledge Submission invalid, they have the option to reject it and furnish reasons, which will then be communicated to the Knowledge Contributor. In the affirmative, proceed to ST 0.1.6 to notify the Knowledge Contributor of the rejection reason. In the negative, move on to ST 0.1.11 to edit the Knowledge Submission. | Knowledge Expert |
| ST 0.1.11 | Edit Knowledge Submission and notify Contributor | Include remarks or additional details with the Knowledge Submission in preparation for subsequent review and approval. Inform the Knowledge Contributor if any changes have been made. Proceed to ST 0.1.12 for the Knowledge Manager to conduct a QA review. | Knowledge Expert |
| ST 0.1.12 | Perform QA Review | The Knowledge Manager conducts a last assessment of the Knowledge Submission, verifying its alignment with the quality and format standards of other Knowledge Documents. Move on to ST 0.1.13 to determine whether to grant approval for the Knowledge Submission to be published. | Knowledge Manager |
| ST 0.1.13 | Approve Publication? | After ensuring that the Knowledge Submission has undergone essential checks and approvals, the Knowledge Manager will make a decision on whether to publish it. In the affirmative, proceed to ST 0.1.14 to verify the appropriate audience and dates for publication. In the negative, move on to ST 0.1.6 for the Knowledge Analyst to communicate the rejection reason to the Knowledge Contributor. | Knowledge Manager |
| ST 0.1.14 | Confirm publication audience and dates | Verify the suitable audience for the Knowledge Submission and check for any constraints or deadlines linked to its publication. Proceed to ST 0.1.15 for the publishing step. | Knowledge Manager |
| ST 0.1.15 | Publish | Release the Knowledge Submission to the Knowledge Base. The 'Contribute and Approve Knowledge' process concludes. | Knowledge Manager |


### Retrieve, Explore, and Apply Knowledge Document (Process ST 0.2).
The Knowledge Base serves as the central storage for the Knowledge Management system. Service Manager offers robust search and retrieval capabilities, enabling users to access, retrieve, and display knowledge documents efficiently. Searches can be conducted using Filters, and the system even supports Boolean searches.

Different types of Knowledge Bases have distinct fields indexed for searching, necessitating the provision of specific search parameters that align with the fields in the knowledge base. For instance, knowledge articles include fields such as title and author. When viewing an incident, the out-of-the-box system presents details like incident number, incident description, and solution for closed incidents.

![enter image description here](https://github.com/QueeNFrisk/KnowledgeManagement/blob/master/contribute_and_approve_km_doc_st7.2%20%282%29.png?raw=true)

| Process ID | Procedure or Decision | Description | Role |
|--|--|--|--|
| ST 0.2.1 | Search Knowledge Base | Input search parameters into the tool. Users can enter search queries either via the Self Service functionality or by Operators from the Interaction, Incident, and Problem Management modules (this is depicted in grey on the process flow as they may not always be present when this process is followed). Proceed to ST 0.2.2 to review the items found. |  Knowledge User|
| ST 0.2.2 | Review Items Found | Examine the search outcomes and ascertain if any are relevant. Proceed to ST 0.2.3 to enhance or modify the search, if needed. | Knowledge User |
| ST 0.2.3 | Refine or change search | If relevant Knowledge Documents have not been retrieved, adjust the search criteria for more accurate results. If affirmative, proceed to ST 0.2.1 to perform another search of the Knowledge Base. If negative, move on to ST 0.2.4 to assess whether relevant Knowledge has been identified. | Knowledge User |
| ST 0.2.4 | Relevant Knowledge Found? | Has a Knowledge Document been provided that is useful and pertinent to the inquiry? In the affirmative, proceed to ST 0.2.6 to Apply Knowledge as appropriate. If negative, move to ST 0.2.5 to decide whether to log an Interaction. | Knowledge User |
| ST 0.2.5 | Log Interaction? | If an appropriate Knowledge Document was not located, it may be necessary to initiate an Interaction to address the researched issue. If affirmative, proceed to Interaction Management (SO 0.1.1). If negative, the 'Search, View, and Utilize Knowledge' process concludes. | Knowledge User |
| ST 0.2.6 | Utilize Knowledge (where appropriate) | Utilize the Knowledge as relevant. Proceed to ST 0.2.7 to decide whether to offer feedback on the Knowledge Document. | Knowledge User |
| ST 0.2.7 | Provide feedback on Knowledge Use? | Feedback is observed for critical factors like the quality and accessibility of the Knowledge Documents. In the affirmative, proceed to ST 0.2.8 to input Knowledge feedback. If negative, the 'Search, View, and Utilize Knowledge' process concludes. | Knowledge User |
| ST 0.2.8 | Populate Knowledge feedback | Provide feedback on the utilized Knowledge Document. The 'Search, View, and Utilize Knowledge' process concludes. | Knowledge User |

### Sustain and consistently enhance Knowledge (Process ST 0.3).
The Maintain And Continually Improve Knowledge process:
-   Records the details of new knowledge (documents)
-   Updates existing knowledge (documents) where there is any inaccuracy or incompleteness
-   Removes obsolete knowledge (documents)

The process is performed by the Knowledge Contributor, Knowledge Analyst, Knowledge Expert, or Knowledge Manager.

| Process ID | Procedure or Decision | Description | Role |
|--|--|--|--|
| ST 0.3.1 | Produce / distribute KM reports | Generate and share KM reports with the Knowledge Manager. Proceed to ST 0.3.2 for the Knowledge Manager to examine the KM reports. | Knowledge Analyst |
| ST 0.3.2 | Review KM reports | Examine the reports for any problems with the tool or process. Proceed to ST 0.3.3 to identify necessary actions. | Knowledge Manager |
| ST 0.3.3 | Actions required? | Determine if there are any further actions required. If affirmative, proceed to ST 0.3.4 to coordinate or perform the necessary actions. If negative, the 'Maintain and Continually Improve Knowledge' process concludes. | Knowledge Manager |
| ST 0.3.4 | Co-ordinate / perform actions | Examine the noted actions and address those that don't necessitate involvement from Knowledge Contributors or Knowledge Experts. Move on to ST 0.3.5 to decide if action is required by the Knowledge Contributor. | Knowledge Analyst |
| ST 0.3.5 | Contributor action required? | In case of an affirmative response, proceed to ST 0.3.6 for the Knowledge Contributor to carry out the necessary actions. If the answer is negative, go to ST 0.3.7 to assess whether action is needed from a Knowledge Expert. | Knowledge Analyst |
| ST 0.3.6 | Perform required actions | Take suitable measures to address the problem identified in the KM report. Proceed to ST 0.3.7 to assess whether action is needed from a Knowledge Expert. | Knowledge Contributor |
| ST 0.3.7 | Expert action required? | If affirmative, proceed to ST 0.3.8 for the Knowledge Expert to carry out the necessary actions. If negative, move on to ST 0.3.9 to decide whether to revise the Knowledge Document. | Knowledge Analyst |
| ST 0.3.8 | Perform required actions | Take necessary actions to address the issue identified in the KM report. Proceed to ST 0.3.9 to decide whether to amend the Knowledge Document. | Knowledge Expert |
| ST 0.3.9 | Revise Knowledge Document? | If affirmative, proceed to ST 0.1.1 for the Knowledge Contributor to input Knowledge details. Note: In this scenario, the role of the Knowledge Analyst is assumed by the Knowledge Contributor. If negative, go to ST 0.3.10 to assess whether to retire the Knowledge Document. | Knowledge Analyst |
| ST 0.3.10 | Archive Knowledge Document? | If affirmative, proceed to ST 0.3.11 to retire the Knowledge Document. If negative, move on to ST 0.3.12 to provide a progress report on the actions. | Knowledge Analyst |
| ST 0.3.11 | Retire Knowledge Document | Store the Knowledge Document in the archive to make it unavailable in searches of the Knowledge Base. Proceed to ST 0.3.12 to provide a progress report. | Knowledge Analyst |
| ST 0.3.12 | Report on progress | Offer the Knowledge Manager a progress update on any pending actions. Proceed to ST 0.3.13 for the Knowledge Manager to assess progress or success. | Knowledge Analyst |
| ST 0.3.13 | Review progress/success | Assess the advancement of identified actions and decide if any further actions are necessary. Proceed to ST 0.3.3 to determine the need for additional actions. | Knowledge Manager |


