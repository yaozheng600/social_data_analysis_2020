# social_data_analysis_2020
## ABSTRACT
### research questions       
Since August 2018, Greta Thunberg, a Swedish environmental activist has become the leader of the global youth anti-climate change movement in just a few months. She is known for conducting the "Skolstrejk för klimatet" (School strike for climate) action outside the Swedish parliament in order to raise global awareness of global warming and climate change issues and speaking at COP24. She was nominated as a candidate for the 2019 Nobel Peace Prize. On March 15, 2019, an estimated 1.4 million students around the world participated in the strikes and protests initiated by her. The huge social influence has earned Tomberg a series of honors and awards. It has also attracted a lot of controversy and criticism, such as “climate protection paranoia”, “climate activists using children for political propaganda”, and “questioning some of her behavior Not environmentally friendly”, etc. Therefore, the main questions we want to know are: 
1. What are the attitudes of netizens towards the climate change campaign led by Thunberg? 
2. What are the hot issues discussed by netizens? 
3. How many percent of people support and oppose Thunberg?
4. Have these attitudes changed over time?
### material and data
We choose youtube as the main social media platform. Select several representative videos as analysis material.
1. In November 2018, she gave a speech at TEDxStockholm. The video has 2,761,996 views and 8,481 comments:[School strike for climate - save the world by changing the rules | Greta Thunberg | TEDxStockholm](https://www.youtube.com/watch?v=EAmmUIEsN9A)
2. On December 12, 2018, she spoke at the 24th United Nations Climate Change Conference on Climate Change (COP24). This video has 1,941,036 views, but comments have been closed:[Greta Thunberg full speech at UN Climate Change COP24 Conference](https://www.youtube.com/watch?v=VFkQSGyeCWg)
3. In January 2019, she was invited to give a speech at the World Economic Forum in Davos. The video has been viewed 204,105 times, but the comment has been closed:[Greta Thunberg: Our House Is On Fire! | World Economic Forum 2019](https://www.youtube.com/watch?v=M7dVF9xylaw)
4. On September 23, 2019, Tumberg delivered a speech at the 2019 United Nations Climate Action Summit in New York, criticizing the countries' insufficient efforts to reduce emissions: "How dare you!" The video has 4,004,566 views, but comments have been closed:[WATCH: Greta Thunberg's full speech to world leaders at UN Climate Action Summit](https://www.youtube.com/watch?v=KAJsdgTPJpU)
5. At the end of 2019, the documentary "I Am Greta". The video has 207,704 views and 1,187 comments:[I Am Greta • Trailer (Official) • A Hulu Original Documentary](https://www.youtube.com/watch?v=xDdEWkA15Rg)      

These videos are Thunberg's several influential events. Except for the documentary, these videos themselves do not contain any subjective opinions to influence the audiences. The Documentary is an important source of data for our summary analysis. Regarding the comments closure problem of some videos, we will analyze the data of some video transport channels instead of official channels.
### technology and methods
Regarding the research questions and material, we propose the following technical methods:
1. Data crawler. Multiple URLs can be crawled, and we can perform an overall analysis of all the crawled comments. We can set a threshold to filter the number of likes and select more useful comments. We can add ip proxy pool to avoid ip blocked issue.
2. Use the naive Bayes classifier to classify positive and negative comments, and calculate the proportion of positive and negative comments.
3. Segment the comments and filter out the most frequent words.
4. Use Altair to visualize the research results.
### analytical approach
In general, we will use the following three approaches to filter out the irrelative comments and make sure the data for analyzing can best represent the audiences' attitude toward videos themselves instead of other topics. 

1. The precautionary approach: When studying the social media controversy, the comments centered on 'home school', 'online school', 'assay' etc. should be filtered out at first, since it is irrelative to the target problem. Any type of bot related actions was not identified.

2. The affirmative mode: YouTube filters popular comments and sorts them according to the number of likes and dislikes, which allows us to filter out valuable information simply and directly. And comments with a large number of responses are usually more controversial arguments. And these replies not only debate existing arguments but also generate new arguments, which expands the scope of discussion.

3. The empirical approach: We should also do the same towards the comments with less than (maybe) 3 letters. This will help filter interfering signals like 'gg' or 'wow'.
