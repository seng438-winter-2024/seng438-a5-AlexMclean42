**SENG 438- Software Testing, Reliability, and Quality**

**Lab. Report \#5 – Software Reliability Assessment**

| Group \#:       |   |
|-----------------|---|
| Dominic Gartner  |   |
| Noel Thomas                |   |
| Alex Mclean                |   |
| Hamd Khan                |   |

# Introduction

# 



# Assessment Using Reliability Growth Testing

For our assessment, we selected the CDS.DAT file. For compatibility with C-SFRAT, we converted it to a CSV, and included certain (inconsequential) fields. This is stored as DATA.csv at the root of this directory.

![](./report-media/data_upload.png)


### Result of model comparison (top two models)
We selected the truncated logistic and IFR generalized Salvia and Bollinger models based on the log-likelihood. This tells how close the model generated curves are to the actual data points. Furthermore, the mean and median critic scores for each of these models were the highest of all tested models. We double checked with a qualitative analysis of the graphs.

![](./report-media/all_model_results.png)

![](./report-media/model_comparison.png)

![](./report-media/selected_model_results.png)


### Result of range analysis
After careful examination of the fault graph and considering the quality and characteristics of the data presented, we have decided to utilize the entire range of data for our analysis. The data quality has been assessed as high, with no significant reasons to suspect inaccuracies or errors. Moreover, the dataset represents the system's performance during its operational phase, which is crucial for understanding its actual reliability in a real-world context. Given that there are no apparent outliers and anomalies, it is justifiable to include the full spectrum of data. This comprehensive approach ensures that we take into account all available information, thereby providing a holistic view of the system's reliability throughout its timeline.

## Plots for failure rate and reliability of the SUT

# ADD ME HERE!! (DELETE ME)

## Discussion on decision making given a target failure rate

# ADD ME HERE!! (DELETE ME)

## Advantages and disadvantages of reliability growth analysis
### Advantages
- **Tracking Bugs in Pre-release**: Reliability Growth Analysis allows for the tracking and identify of bugs or reliability issues during the pre-release phase of product development. By analyzing trends in failure data over time, we are able to detect and address potential issues early, leading to improved product quality and reduced post-release defects!
- **Guiding Software Testing Process**: Reliability Growth Analysis serves as a valuable tool for guiding the software testing process. By monitoring the trend of failure data and analyzing reliability metrics, we can pick and choose specific testing strategies and prioritize testing efforts based on identified reliability issues. This can speed up the testing process and allows for better testing coverage, which enhances the overall quality of the software!
- **Releasing the Product**: Reliability Growth Analysis aids in making informed decisions about releasing the product to the market. This helps mitigate the risk of releasing a potentially unreliable product, thereby safeguarding the organization's reputation and customer satisfaction!
### Disadvantages
- **Resource Intensive**: We noticed that Reliability Growth Analysis can be resource-intensive, which can require a significant amount of time and effort. Additionally, Reliability Growth Analysis requires a lot of data collection, analysis, and interpretation, which also can require a significant amount of time and effort.
- **Complexity of Data Analysis**: We also noticed that in reliability growth analysis there is a lot of complex data analysis and math involved. Additionally, the selecting of an appropriate model can also cause difficulties.

# Assessment Using Reliability Demonstration Chart 
Datachosen --> CRS3.Data

Smallest MTTFMin before not being acceptable = 0.087 

### MTTFmin Chosen = 0.087

![](./report-media/mainmttf.png)

### 2 X MTTFmin Chosen = 0.174
![](./report-media/full.png)

### 1/2 X MTTFmin Chosen = 0.0435

![](./report-media/half.png)


# 

# Comparison of Results
1. **Similarities:**
    - Both techniques aim to assess the reliability of the system under test.
    - They involve analyzing failure data to make informed decisions about the system's reliability.
2. **Differences:**
    - Reliability growth testing focuses on analyzing the trend of failure data over time to assess improvements in reliability during testing phases.
    - RDC, on the other hand, assesses reliability based on cumulative failure observations and is particularly useful when failure data is limited and time of failures is known.
    - The techniques use different tools and methodologies for analysis (C-SFRAT for reliability growth testing and RDC for reliability demonstration chart).

In summary, while both techniques serve the purpose of reliability assessment, they differ in their approaches and methodologies. Reliability growth testing focuses on improvements over time, while RDC provides a snapshot assessment based on cumulative failure observations. The choice of technique depends on factors such as the availability of data and the stage of testing or operation of the system.


# Discussion on Similarity and Differences of the Two Techniques





# How the team work/effort was divided and managed
As a team, we decided to split the work by sections. Two members worked on the first part of the lab on "Reliability Growth Testing" while the other two members worked on the second part on "Assessment using reliability demonstration chart". Once both parts were completed, all members reviewed the work of others, and gave feedback if needed. This divided the work load between team members, while achieving effective progress. 

# Difficulties encountered, challenges overcome, and lessons learned
Throughout this assignment, we did not face any major challenges as a group. But we had a lot of difficulties encountered with trying to download the C-SFRAT and running the data on it. As everyone in the group had mac's it was a lot harder to run and use the program! We tried may different virtual machines, which included: 
- University of Calgary's Windows 10 VMware Horizon Client (Didn't work as they don't have Java installed, and don't let you run .exe files without admin approval) 
- UTM Windows VM (We were not able to create an instance what wouldn't crash when trying to login to windows)
- University of Calgary's own computers (Didn't work as they don't have Java installed, and don't let you run .exe files without admin approval)

We ended up getting it working using Azure's VM, but this entire process was such a pain to over come. Maybe it might have been easier to use a different growth testing software... (If we did this lab again...)

# Comments/feedback on the lab itself
Other then the major challenge faced above, we really enjoyed this lab, it was helpful getting us familiar with the growth testing process, and using some concepts we learned in class in a real time environment. We found the lab document itself great and very easy to understand. Furthermore, the lab structure allowed for effective learning of testing methodologies and signified the importance of testing in a variety of methods.
