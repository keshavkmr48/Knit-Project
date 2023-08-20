# Knit-Project
Create a chatbot that can take natural language input from user and produce output data and chart as insights for the customer survey data.

### Problem Statement
 Data analysis for surveys is a fairly manual, time-consuming process. Market researchers conducting surveys need to create crosstabs (pivot tables), charts, filter the data by segments, and more, to uncover the insight behind the data so that they can tell a powerful story to their stakeholders and make decisions.

 ### Solution 

 This project focuses on solving this critical issue by developing an MVP of a chatbot agent that can engage with market researchers or other stakeholders in a natural language dialogue. The chatbot will provide insights, statistics, and charts based on survey responses, making the process of interpreting and understanding survey results efficient and user-friendly.


 ### Task to Accomplish 

 Given a DataFrame containing survey response data and a JSON file detailing the survey questions with their type, mapped to question IDs (that are column names in the DataFrame). Your task is to design a solution that can interpret natural language queries/questions about this survey data and return relevant answers.

 ## Evaluation Criteria 

- User-Centric Approach: How well does your solution consider the needs of the end-users (market researchers)? How effectively does it provide them with meaningful insights into the data?
    #### Points 
    - End-User should be able to study survey data at multiple levels in Top-2-Down Approach. Few of the High Level Insights about data should come automatically once the data is uploaded.

        **Level-01 : Survey Response Meta Data (Auto-Generated)**\
            Example:- \
            Total Number of Survey Participants, % of participants with complete responses,\
            % of responses for each questions, Top 5 questions answered, Least 5 questions answered. \
            This will help in setting up the context for analysing the response of the survey for business insights. 

        **Level-02 : Business Metrics (Quant & Qual) captured through data (Configurable/Manual/Auto-Generated)**\
        **Level-03 : Drilling Down, Investigation and Understanding Relationship (Manual)**
    - Results and Insights should be less verbose and more visual.
    - All Queries and the Results (Entire Interaction) should be downloadable/transferable as PPT in Question-Answer Pair.
         

- Functionality: Does the chatbot accurately respond to user queries and provide relevant statistics and charts?
    #### Points
    - If the data processing step done well, and column names of the final data frame have appropriate context, chatbot responds to the user query considerbaly well. 
- Innovation: Is the approach creative, utilizing the recommended technologies in an effective manner?
  #### Points
  Yes, the recommended technology have been used judiciously, creatively and customized to the problem at hand.
- Vision and Future Improvement: How well have you thought about the potential areas for improvement, scalability, and          alignment with long-term vision?
  #### Points
  - We need to automate the data processing part using multi-prompt, user defined fucntions as tools and router chain stacking multiple chains, each corresponding to individual question types - single choice, multi-choice, single -matrix and rank order.
  - To convert it into a full blown application, we can configure this at user level in the application and then at dataset level for session and provide the llm with appropriate memory (mostly, conversation summary).
