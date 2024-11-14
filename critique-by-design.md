| [home page](https://cmustudent.github.io/tswd-portfolio-templates/) | [visualizing debt](visualizing-government-debt) | [critique by design](critique-by-design.md) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Critique by Design with Tableau (MakeoverMonday) 

## Step one: the visualization

[Link to Original Data Vizualization](https://www.nytimes.com/2020/02/06/learning/whats-going-on-in-this-graph-engagement-ring-costs.html)

![image](https://github.com/user-attachments/assets/5b3a257f-0549-4c95-bc1a-88dd7a519423)

I chose the original visualization because I’ve always been intrigued by how people approach big purchases like engagement rings, especially when it comes to balancing cost with personal significance. Seeing spending patterns alongside income data gave me a unique perspective on the financial sacrifices people might make for these meaningful items. I found it fascinating how different income levels impact not only what people spend but also how long it would take them to save for such a purchase, shedding light on the real financial weight of an engagement ring.

## Step two: the critique

1. Introduce Subtle Color Variation by Income Bracket: Adding a gradient or color variation based on income bracket could help viewers quickly discern patterns across income levels without needing to rely on legend references. This small change would improve perceptibility and add another layer of insight without cluttering the visualization.
2. Add a Contextual Benchmark or Reference Line: Including a benchmark line, such as the average national engagement ring cost or the historical average, would provide context for viewers. This addition would enhance completeness by allowing the audience to see how current spending aligns with or deviates from typical values, helping them make better-informed comparisons.
3. Incorporate Annotations to Highlight Key Insights: Use short text annotations directly on the chart to highlight data points of interest, such as “Most common spending range is under $1k,” or “Higher-income groups spend less proportionally”


## Step three: Sketch a solution

![image](https://github.com/user-attachments/assets/ab590c54-2a73-4eaa-9cc5-3f2c003694ff)
![image](https://github.com/user-attachments/assets/6fccbf7e-3823-44d8-8122-e921c9bd6020)

The vizualization I chose was already quite good so, I tried to incorporate the above critiques, to improve it further.


## Step four: Test the solution


| Question | Interview 1 | Interview 2 |
|----------|-------------|-------------|
|Can you tell me what you think this vizualization aims to depict? | These look like a charts that show how many people are spending different amounts on engagement rings. The bars are higher on the left side, which might mean that more people spend less on rings.  The other chart shows how long it would take people from different income groups to save up for an engagement ring. The bars go from left to right and are different lengths.           | This looks like a histogram showing how many people spend different amounts on engagement rings, with an “Above Average” and “Below Average” color distinction. The left side has higher bars, which I assume indicates more people are spending in the lower price ranges. This appears to be a horizontal bar chart showing the time (in months) it would take different income groups to save enough money to buy an average-cost engagement ring. It has a gradient that seems to indicate time differences between income categories. |
| Is there anything you find surprising or confusing?| I'm a bit confused by the color usage here because I can’t tell exactly what each color means. The legend says “Above Average” and “Below Average,” but I'm not sure what this is referring to. It would help if there was more explanation. It’s not too confusing, but I’m not sure if the colors mean something special. It would help if the colors were more distinct for someone like me who has trouble seeing them clearly. | While it’s mostly clear, there are a few issues: 1. Color Gradient Ambiguity: The gradient doesn’t add much value here because the color range isn’t associated with any specific meaning in the context of time. It would be better to use a solid color for each bar to avoid ambiguity. 2. Lack of Units in Axis Labels: The X-axis lacks a unit indicator (e.g., “Months”), which could confuse users at first glance. It’s crucial to label the axis clearly to avoid misinterpretation. 3. Missing Context: There’s no clear indication of why these particular income brackets were chosen or how they relate to typical incomes. It might help to add context about how average engagement ring prices compare to average income levels            |
| Are the visualizations hard to understand? Do you need me to explain what the visualizations are for? | Yes, I could use some clarification. I understand it’s about how much people spend on rings, but the meaning of the colors and the significance of "average" could be clearer. This one is easier to understand than the first chart, but an explanation about why this information is important would help. Also, clearer labeling would make it more accessible. | The visualization communicates the general trend well enough, but it’s harder to get precise insights without improvements. For an informed audience, the purpose is relatively clear, but for a general viewer, the lack of direct labeling, ambiguous color usage, and absence of an average reference line make it less effective than it could be. The chart is fairly intuitive, but the color gradient and lack of units on the X-axis reduce its clarity. A short explanatory note would make the intent clearer and prevent any initial confusion. |
| Who do you think is the intended audience? | This seems like it might be for people who want to understand spending habits on engagement rings, maybe those in the jewelry business or people researching spending trends. It seems like this is for people who are analyzing how much of an impact an engagement ring purchase has on different income groups. Maybe people in finance or researchers studying consumer spending? | It seems like it’s intended for people interested in analyzing spending trends on engagement rings, possibly those in retail, marketing, or consumer research. However, the execution limits its accessibility and usability for a general audience. This visualization seems aimed at people analyzing the financial burden of engagement rings on different income levels. It would be valuable for financial analysts, consumer researchers, or marketing professionals looking to understand affordability. |

Synthesis: 

The feedback highlights several recurring themes across both visualizations:
1. Need for Clearer Labels and Explanations: Both viewers emphasized the importance of direct labeling, especially around axes, units, and any significant reference points (like the average line). Ambiguous terms like "Above Average" and "Below Average" need context to avoid misinterpretation.
2. Color Choices and Accessibility: Color usage was a concern in both visualizations. For the first intervieww, the colors used were not distinct enough, while the UX designer pointed out that the color choices lacked intuitive meaning and clarity. Both perspectives suggest that the colors should be more meaningful and accessible.
3. Desire for Reference Points and Context: Both viewers felt that the absence of an average line in the histogram and contextual information in the income-based chart made it harder to understand the full story. Adding these reference points would anchor the data and make the insights more interpretable.
4. Simplification of Visual Elements: There was feedback on reducing unnecessary visual complexity, such as the use of gradients in the income chart and abbreviations on the X-axis in the histogram. Both viewers preferred simpler, more straightforward visuals that emphasize readability.


## Step five: build the solution

Based on the feedback, the following design changes would enhance clarity, accessibility, and user experience:
1. Add Direct Labels and Units:
  - Histogram: Label each bar with the exact number of people to reduce the need to interpret the Y-axis. Spell out full numbers on the X-axis (e.g., "$1,000" instead of "1K") to improve readability.
  - Income Chart: Label the X-axis with units ("Months") and use a title that clarifies the purpose of the chart (e.g., "Months Required to Save for an Average Engagement Ring by Income Level").
2. Use Accessible and Intuitive Colors:
  - Replace the orange and yellow colors in the histogram with a more color-blind-friendly combination, such as blue for "Below Average" and red for "Above Average." This will create a clearer contrast and make the "Above/Below Average" distinction more intuitive.
  - In the income chart, replace the gradient with solid colors for each bar to avoid ambiguity. Alternatively, use distinct shades for each income bracket to provide subtle differentiation without confusion.
3. Add Reference Lines and Contextual Annotations:
  - Income Chart: Add a brief annotation explaining why certain income levels might need more or fewer months to save. For example, a short note could clarify that lower-income earners need a longer time to save up due to a higher income-to-cost ratio.

[![Cost of Engagement Ring](https://public.tableau.com/static/images/De/Desai_Amogh-Engagement_Ring1/Sheet1/1_rss.png)](https://public.tableau.com/views/Desai_Amogh-Engagement_Ring1/Sheet1)

[![Time to Buy Engagement Ring by Income Brackets](https://public.tableau.com/static/images/De/Desai_Amogh-Engagement_Ring2/Sheet1/1_rss.png)](https://public.tableau.com/views/Desai_Amogh-Engagement_Ring2/Sheet1)


