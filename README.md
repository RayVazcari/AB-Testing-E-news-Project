<h1><center><font size=10>Data Science and Business Analytics</center></font></h1>
<center>Project 2 - Business Statistics: E-news Express</center></h1><p
<center>Jorge Ramon Vazquez Campero</center></h1>

**`| Hypothesis Testing | A/B Testing | Data Visualization | Statistical Inference | Exploratory Data Analysis | Variable Identification | Univariate Analysis | Bi-Variate Analysis | Advanced Python techniques | Insights Generation |`**

This project used statistical analysis, A/B testing, and visualization to decide whether the new landing page of an online news portal (E-news Express) is effective enough to gather new subscribers. The simulated dataset includes important metrics such as conversion status and time spent on the page, which help in concluding the effectiveness of the new landing page. Additionally, the dependence of conversion on the preferred language is analyzed in this project. This experience has further solidified my passion for data science and my ability to draw meaningful conclusions from complex data sets. I look forward to leveraging these insights to drive impactful business solutions. 🚀

   <p align="left"> 
     <a href="https://github.com/RayVazcari?tab=followers">
         <img alt="followers" title="Follow me on Github" src="https://custom-icon-badges.demolab.com/github/followers/RayVazcari?color=236ad3&labelColor=1155ba&style=for-the-badge&logo=person-add&label=Follow me on Github &logoColor=white"/></a>
      <a href="https://www.linkedin.com/in/rayvazcari/">
         <img alt="Linkedin Profile" title="Likedin Profile" src="https://custom-icon-badges.demolab.com/badge/-Linkedin%20Profile-blue?style=for-the-badge&logoColor=white&logo=linkedin"/></a>
      </a>
</p>

---

### 🧰 Languages and Tools I Used on This Project
<img align="left" alt="Jupyter" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/jupyter/jupyter-original-wordmark.svg" />
<img align="left" alt="Maplotlib" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/matplotlib/matplotlib-original.svg" />
<img align="left" alt="Numpy" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/numpy/numpy-original.svg" />
<img align="left" alt="Pandas" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/pandas/pandas-original.svg" />
<img align="left" alt="Plotly" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/plotly/plotly-original.svg" />
<img align="left" alt="Python" width="30px" style="padding-right:10px;"  src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" />
<img align="left" alt="Raspberry Pi" width="30px" style="padding-right:10px;"  src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/raspberrypi/raspberrypi-original.svg" />
<img align="left" alt="VScode" width="30px" style="padding-right:10px;"  src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vscode/vscode-original.svg" />
<img align="left" alt="Seaborn" width="30px" style="padding-right:10px;" src="https://seaborn.pydata.org/_images/logo-mark-lightbg.svg"  /> 
<img align="left" alt="Maplotlib" width="30px" style="padding-right:10px;"  src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/pytorch/pytorch-original.svg" />

<br />

---

<center><img src="https://vignette.wikia.nocookie.net/logopedia/images/1/18/E!_News_2012_Logo.png/revision/latest?cb=20161004214546" width="600" height="300"></center>

<br />

---


### 📊 Project Overview

## Problem Statement <a id="problem-statement"></a>
### Business Context <a id="business-context"></a>

The advent of e-news, or electronic news, portals has offered us a great opportunity to quickly get updates on the day-to-day events occurring globally. The information on these portals is retrieved electronically from online databases, processed using a variety of software, and then transmitted to the users. There are multiple advantages of transmitting news electronically, like faster access to the content and the ability to utilize different technologies such as audio, graphics, video, and other interactive elements that are either not being used or aren’t common yet in traditional newspapers.

E-news Express, an online news portal, aims to expand its business by acquiring new subscribers. With every visitor to the website taking certain actions based on their interest, the company plans to analyze these actions to understand user interests and determine how to drive better engagement. The executives at E-news Express are of the opinion that there has been a decline in new monthly subscribers compared to the past year because the current webpage is not designed well enough in terms of the outline & recommended content to keep customers engaged long enough to make a decision to subscribe.

### Objective <a id="objective"></a>

The design team of the company has researched and created a new landing page that has a new outline & more relevant content shown compared to the old page. In order to test the effectiveness of the new landing page in gathering new subscribers, the Data Science team conducted an experiment by randomly selecting 100 users and dividing them equally into two groups. The existing landing page was served to the first group (control group) and the new landing page to the second group (treatment group). Data regarding the interaction of users in both groups with the two versions of the landing page was collected. Being a data scientist in E-news Express, you have been asked to explore the data and perform a statistical analysis (at a significance level of 5%) to determine the effectiveness of the new landing page in gathering new subscribers for the news portal by answering the following questions:

1. Do the users spend more time on the new landing page than on the existing landing page?

2. Is the conversion rate (the proportion of users who visit the landing page and get converted) for the new page greater than the conversion rate for the old page?

3. Does the converted status depend on the preferred language? [Hint: Create a contingency table using the pandas.crosstab() function]

4. Is the time spent on the new page the same for the different language users?

### Data Dictionary <a id="data-dictionary"></a>

The data contains information regarding the interaction of users in both groups with the two versions of the landing page.

1. **`user_id`** - Unique user ID of the person visiting the website
2. **`group`** - Whether the user belongs to the first group (control) or the second group (treatment)
3. **`landing_page`** - Whether the landing page is new or old
4. **`time_spent_on_the_page`** - Time (in minutes) spent by the user on the landing page
5. **`converted`** - Whether the user gets converted to a subscriber of the news portal or not
6. **`language_preferred`** - Language chosen by the user to view the landing page

---

### Summary of Findings

1. **Do the users spend more time on the new landing page than on the existing landing page?**
   - **T-test Results:**
     - Average time on the new landing page: 6.22 minutes
     - Average time on the old landing page: 4.53 minutes
     - T-test statistic: 5.88
     - P-value: < 0.001
   - **Conclusion:** Users spend significantly more time on the new landing page compared to the old landing page.

2. **Is the conversion rate for the new page greater than the conversion rate for the old page?**
   - **Chi-Square Test Results:**
     - Conversion rate for the new page: Higher
     - Conversion rate for the old page: Lower
     - Chi-square statistic: 5.89
     - P-value: 0.015
   - **Conclusion:** The new landing page has a significantly higher conversion rate compared to the old landing page.

3. **Does the converted status depend on the preferred language?**
   - **Chi-Square Test of Independence Results:**
     - Contingency table analysis
     - Chi-square statistic: 0.85
     - P-value: 0.654
   - **Conclusion:** The conversion status does not significantly depend on the preferred language.

4. **Is the time spent on the new page the same for the different language users?**
   - **ANOVA Test Results:**
     - Average time for English users: 6.5 minutes
     - Average time for Spanish users: 6.2 minutes
     - Average time for French users: 6.0 minutes
     - F-statistic: 0.85
     - P-value: 0.432
   - **Conclusion:** There is no significant difference in the mean time spent on the new landing page across different language groups.

### Business Recommendations

1. **Launch New Landing Page:**
   - I would recommend implementing the new landing page in view of the significant increase in both time spent and conversion rate. Indeed, this is likely to be more effective in engaging users and hence increase the subscription rate.
   - Above-average times may suggest that users stay on the new landing page because of better content or layout, respectively.
   - Even optimize its layout and content so that greater engagement can be achieved. Monitor time taken by users in different sections and work on it to keep the content fresh and engaging.

2. **Track User Involvement:**
   - Continue to watch user engagement metrics like time spent and conversion rates. Make sure that the same new landing page continues to be effective over time. Regular A/B testing can help in making iterative improvements.

3. **Language-Specific Customizations:**
   - Inasmuch as the status of conversion did not depend on the preferred language, and the close time spent under different languages indicates an almost identically long interaction with the platform, so there is no urgent need to introduce some language-dependent adjustments. However, diving deeper and analyzing the conversion rates for other segments, like language or user demographics, could be informative as to which specific sub-groups are more likely to convert, allowing further customization of marketing efforts or user experience improvements.
   - Use insights gained from univariate and bivariate analyses for targeted marketing campaigns. For example, if it appears that some specific language groups or user demographics have more engagement or conversion, then the message for those marketing segments should be fine-tuned in order to have a bigger effect.

4. **Data-Driven Decision Making:**
   - Encourage a data-driven culture in making decisions within the organization. Very nice results from this A/B test, which lends weight to the fact that business statistics back up the decisions we make.

5. **User Feedback and Qualitative Research:**
   - For a fuller picture, qualitative research with users, like user surveys or interviews, can be aligned with the more objective numbers from quantitative analysis to understand their user preferences and pain points properly. This approach helps in understanding more deeply the reasons why particular elements work, and how they can be built on effectively.

