# Netflix-Titles-Evaluation

This Power BI report provides a concise evaluation of Netflix titles, designed to offer actionable insights for content strategists, marketing, and executives. It leverages data preparation and advanced analytics to understand content trends and inform strategic decisions.


Report Page Stories and Key Insights
The report is structured into three pages, each telling a vital part of the Netflix content story:
Overview:
This page gives an immediate grasp of Netflix's content scale, showing the total number of titles and their year-over-year growth. It highlights the distribution between Movies and TV Shows and the top genre categories by title count, quickly assessing content investment and library composition.
Geographic Distribution:
This section reveals Netflix's global presence through country-wise title availability and analyzes historical release patterns to show content growth over time. It also identifies seasonal trends in content additions and the strategic balance between co-productions and stand-alone productions, reflecting international collaboration efforts.
Audience & Production Insights:
This final page explores content rating distribution to understand target audiences. It spotlights top directors by title count, highlighting key creative partners, and further clarifies Netflix's co-production vs. stand-alone strategy, indicating its global partnership and domestic focus.

Key Technical Challenges Successfully Overcome
Throughout this project, specific technical obstacles were encountered and effectively resolved, demonstrating robust problem-solving and Power BI expertise:
Deconstructing Multi-Valued Fields: The genre and country columns presented a core challenge, holding multiple, comma-separated values within a single cell. This was successfully addressed by implementing Power Query's "Split Column by Delimiter" with the "Split into Rows" option, a crucial step for granular, individual analysis of each genre and country.
Ensuring Accurate Counting Post-Transformation: A direct consequence of expanding rows from multi-valued fields was the potential for inflated counts across the dataset. This was systematically mitigated by consistently applying DISTINCTCOUNT( ) in all title-counting DAX measures, guaranteeing that each unique title was precisely counted regardless of data duplication.
Developing Dynamic Production Type Classification: Classifying titles as either "Co-Production" or "Stand-Alone Production" required a sophisticated DAX solution. This was achieved by crafting a calculated column utilizing CALCULATE in conjunction with ALLEXCEPT to accurately count distinct countries per show id, thereby providing a robust, context-aware method for categorization and subsequent comparative analysis within the expanded dataset.

Conclusion & Recommendations
This report is a powerful tool for data-driven decisions on content acquisition, production, and market expansion. Future enhancements could include integrating viewership data, sentiment analysis, competitive benchmarking, and advanced parameterization for deeper strategic insights. The project has profoundly honed analytical and visualization skills.
