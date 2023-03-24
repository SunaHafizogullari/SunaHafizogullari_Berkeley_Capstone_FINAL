### Leveraging Student Information to Enhance College Persistence

Suna Hafizogullari

#### Executive summary
10,000 Degrees is dedicated to empowering students from economically disadvantaged backgrounds to succeed in college through comprehensive support and scholarship opportunities. With a remarkable four-year college graduation rate of 80%, significantly higher than the national average of 31%, the organization has demonstrated a proven track record of success. This study sheds light on the data collected from participants in 10,000 Degrees programs, obtained through the National Student Clearinghouse (NSC), to further deepen our understanding of the organization's impact.

The purpose of this study is to pinpoint the students who face an increased likelihood of leaving college, uncover the underlying factors that contribute to their decision, and furnish 10,000 Degrees with actionable insights to intervene before student attrition takes place. 

#### Rationale
Education equity is a foundation for strengthening the economic vitality and social health of all communities. By furnishing 10,000 Degrees with data-driven insights, we can aid the organization in its efforts to proactively identify and support at-risk students.

#### Research Question
The main objectives of this research are to:

- Develop a predictive analytics scoring system that ranks students' likelihood of persisting to their second year of college within the 10,000 Degrees program
- Identify key factors that impact student persistence
- Assist 10,000 Degrees in integrating the scoring system into their decision-making process.
- Utilize data insights to continually improve the accuracy and effectiveness of the scoring system

#### Data Sources
The student data is provided by 10,000 Degrees and obtained through the National Student Clearinghouse (NSC), and includes the following:

- Demographics data such as gender, race/ethnicity, English as a second language, and highest degree earned before starting college
- High school data such as name, region, graduation year, participation in the 10,000 Degrees program, and dual enrollment during high school
- College data such as name, region, 2 year vs. 4 year program, participation in the 10,000 Degrees program, persistence indicator for the second year of college (target variable), and transfer status to a 4 year college
- Publicly available data sources include:
- GreatSchools.org for school ratings
- County information for residence

#### Methodology
Classification techniques were employed to determine the students who are facing obstacles in their academic journey and the specific factors that are hindering their success.

#### Results
After testing several models on the analysis sample, the gradient boosting model was chosen due to its superior performance on both the training and test samples.

The following observations were made based on the model's ability to rank students by their probability of dropping out of college:

- The chart provided below offers valuable insights into the model's performance. It reveals that students in the top deciles are considerably more likely to drop out than those in the lower deciles.
- On the training sample, the dropout rate for the highest scoring decile is over nine times greater than that for the lowest scoring decile. - The gap between these two groups is much smaller on the test sample but still noteworthy, with a dropout rate of 65% versus 20%.
- The dropout rates show no fluctuations in the training sample, indicating a perfect rank ordering of the score. The fluctuations are minimal for the test sample as well, further indicating the model's reliability.

Based on our analysis, the likelihood of a student persisting to their second year of college is most strongly influenced by the following top five factors:

- Participation in a summer program offered by their college after high school graduation
- Attending a high school with a high rating
- Enrollment in a Success program with a scholarship
- Race
- Geographic location of the college attended

#### Future reseach
We're actively collaborating with 10,000 Degrees to improve our model's performance by addressing some critical areas:

- To increase the sample size, we are working with 10,000 Degrees to retrieve the persistence status of the excluded students with Persistence Indicator = 'Ineligible'. These students didn't start college right after high school and did not receive a Yes/No value for Persistence Indicator. 10,000 Degrees is collaborating with their partner who flattens the NSC data to explore alternative ways of obtaining their persistence status. If we can get a valid Persistence Indicator for these students, we can possibly double our data size and enhance our analysis.
- The Success program participation factor needs to be further investigated as there are indications that the students who didn't attend the program have lower persistence rates. We'll be closely working with 10,000 Degrees to identify the underlying reasons.
- Another crucial aspect we're exploring is the impact of full-time student status on persistence rates. 10,000 Degrees' prior research suggests that full-time students are more likely to persist, and we're trying to access this data to improve our model.
- We also plan to isolate the COVID-19 period in our analysis and compare the model's results with and without the pandemic data once we have a bigger sample. This will help us gain more insights into the factors affecting student persistence during challenging times.
- As we work to expand our data sample, we may want to explore other modeling techniques such as neural networks. While the gradient boosting model has shown promise, we are interested in evaluating whether a neural network could lead to further improvements in our predictive performance.
- It's important for our model to be interpretable so that we can provide meaningful insights to 10,000 Degrees. To that end, we will research how to build more explainable models and explore ways to provide detailed explanations at the individual record level to better understand the factors impacting a student's persistence score.

#### Outline of project

- [Link to Notebook 1 for Part 1: Exploratory Data Analysis](https://github.com/SunaHafizogullari/SunaHafizogullari_Berkeley_Capstone_FINAL/blob/main/Part%201_Exploratory%20Data%20Analysis.ipynb)
- [Link to Notebook 2 for Part 2: Model Development and Validation Results Using Traditional ML Algorithms](https://github.com/SunaHafizogullari/SunaHafizogullari_Berkeley_Capstone_FINAL/blob/main/Part%202_Model%20Development%20and%20Validation%20Results%20Using%20Traditional%20ML%20Algorithms.ipynb)
- [Link to Notebook 3 for Part 3: Model Development and Validation Results Using Ensemble Algorithms](https://github.com/SunaHafizogullari/SunaHafizogullari_Berkeley_Capstone_FINAL/blob/main/Part%203_Model%20Development%20and%20Validation%20Results%20Using%20Ensemble%20Algorithms.ipynb)
- [Link to Notebook 4 for Part 4: Part 4: Comparison of Model Validation Results](https://github.com/SunaHafizogullari/SunaHafizogullari_Berkeley_Capstone_FINAL/blob/main/Part%204_Comparison%20of%20Models.ipynb)
- [Linek to Notebook 5 for Part 5: Conclusions](https://github.com/SunaHafizogullari/SunaHafizogullari_Berkeley_Capstone_FINAL/blob/main/Part%205%20_Conclusions.ipynb)

##### Contact and Further Information
E-mail: shafizogullari@gmail.com
