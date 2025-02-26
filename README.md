# IISE_QCRE_Data_Challange_2025
On behalf of the Quality Control & Reliability Engineering (QCRE) community, we would like to invite you to participate in the 2025 QCRE Data Challenge Competition at the IISE Annual Conference. This year's QCRE Data Challenge problem is sponsored by Zauron Labs. The dataset is provided by The University of Texas Medical Branch at Galveston. 

In this data challenge, a research problem of Vertebral Fracture Detection is posed to participants. More details regarding the competition problem statement can be found in the attachment. 

# Eligibility
- Individuals or teams of a maximum of four members.   

- At least one of the team members must be an active member of the Institute of Industrial & Systems Engineers (IISE) and Quality Control & Reliability Engineering (QCRE) division.

- Each team can only participate once.

- Each team should submit a Notice of Intent Form to enter the competition (check details in the Notice of Intent section).

- Completing Steps 1-3 in the Submission section is required for any team to be eligible as a finalist.

- Participating teams are required to publicly release their solutions, including source code and trained model weights, on open-source platforms under the MIT license.

- Finalist teams acknowledge that the competition organizers will publish their technical papers, solutions, source code, and trained model weights on the official competition GitHub page [https://github.com/SHAFNehal/IISE_QCRE_Data_Challange_2025](https://github.com/SHAFNehal/IISE_QCRE_Data_Challange_2025). 
- Participants must not share the challenge data publicly. Instead, they should refer to the original data request link provided by the competition organizers for access and distribution guidelines. 

# Notice of Intent
Each team must submit a Notice of Intent Form by March 7th, 2025, through https://forms.office.com/r/ics3Lx9y6V to express their interest in entering the competition. The data will start to be released to each team on a First Come First Serve. The form requires the following information: Team members, Institution, Main point of contact (name and email address), and Copyright release agreement.

# Submission Guidelines
## Step 1: Initial Submission
Participating teams or individuals must submit the following files to iiseqcredcc@gmail.com and copy all the Chairs of the Competition Steering Committee no later than April 14, 2025:
1.	The source code for model development and training.
2.	The source code for model prediction (“predictions.py”).
3.	The trained model weights.
File Structure

The submitted files should follow the structure below:
    |- DataFile
        |- train_data
        |- test_data
    |- trained_weights
    |- train.py
    |- predictions.py

The primary script for generating predictions must be named “predictions.py”. This script should be capable of directly loading the trained model weights, reading DICOM files from the test_data folder or any other designated held-out test dataset, and producing the corresponding predictions.
It is imperative that the prediction script “predictions.py” runs without requiring any modifications. Any necessary software dependencies should be explicitly stated in the submission. Additionally, a ReadMe file must be included, providing clear instructions on how to execute the code.

## Step 2: Technical Report Submission
All finalists will be required to submit a technical report (not exceeding five pages, excluding references) by May 15, 2025. The report should include the following sections:
-	Team Members: Names, affiliations, and roles.
-	Introduction: Overview of the problem and motivation.
-	Methodology: Description of the approach, models, and techniques used.
-	Data Analysis/Result Discussion: Insights derived from the data and model performance.
-	Conclusions: Summary of findings and implications.

Additionally, the submission email must include:
-	A list of team members, including their full affiliations and contact information (email and phone number).
-	Identification of one team member as the primary contact for the team.

Email your submission Data Competition steering committee. 

## Step 3: Finalist Presentation at the IISE Annual Meeting
Finalist teams must showcase their work at the 2025 IISE Annual Conference & Expo. At least one team member from each finalist team is required to register for the conference and present their technical details during the QCRE Data Challenge Competition showcase session.
For any further inquiries, please contact the Chair of the Competition Steering Committee.

# Evaluation and Selection of Winner
The Competition Steering Committee will assess submissions based on the files specified in Step 1 of the Submission section. Only teams that have submitted all the required files in Step 1 will be considered for evaluation. The evaluation committee will include at least one representative from the data sponsor partner with domain expertise.
The model performance will be measured based on 
Score = Mean Average Precision (mAP)@0.5 
```
mAP@0.5 indicates mean average precision at IoU threshold of 50% for the object detection tasks.
```
Selection Process
- A maximum of four teams with the highest Score will be selected as candidate finalists.
- Finalists will be invited to proceed with Steps 2 and 3 outlined in the Submission section.
- Among the finalist teams, those who successfully complete all three steps will be ranked based on their Score, and the top four teams will be awarded 1st to 4th place prizes accordingly.

For any further questions, participants may reach out to the Competition Steering Committee.


# How to read DICOM files:
PyDicom is a useful python library to read DICOM files and handle data as needed. Please, check the following link for detail usage: https://github.com/pydicom/pydicom


# Q&A for the Challange:
### Q1: Are we allowed to use pre-trained models?
Yes, you are allowed to use any pre-trained model as long as they are available in open domain (e.g., MIT License). 

### Q2: Can we change or add new team members after submitting NoI?
Answer: Yes, you can. But remember the size of the team is capped by 4 members.
