# MOMA-Dashboard-Analysis
This Project involves building an interactive Power BI dashboard using datasets from the Museum of Modern Art On View (MOMA). "On View" refers to artwork that are currently exhibited in the physical gallaries of the Museum of Modern Art. The dashboard provides deep insights into artists, their artworks, and acquisition trends from 1932- 2024.
In this Dashboard, the 'On View' analysis focuses on :
- Number of artworks currently displayed.
- Artists with the most works on View
- Most common classification and mediums on display.
- Trends in artwork acqusition years

# Project Background
The Museum of Modern Art (MOMA) in New York City is one of the world's most influential institutions dedicated to modern and contemporary art. With over 200,000 works from more than 10,000 artists, its collection spans painting, sculpture, photography, design, and more.
This project presents an analysis of over 1000 artworks On View at the Museum to transform raw data into visual narratives that reveals patterns, highlight diversity, and make it easier to understand the museum's collection and curation practices.

# Overview of the Data
The Dataset used in this project was sourced from Maven Analytics. It includes detailed information about the museum's artworks and the artists who created them. The dataset is organized into main tables: 

- ## 1. Artist Table
  Contains information about each artist in the MOMA collection
- Constitutent ID - Unique identifier for each artist.
- Display Name - Full name of the artist.
- Artist Bio - Short biographical note.
- Nationality - Artist's Region.
- Gender - Male, Female, Transgender woman or Unknown.
- Begin Date - Year of Birth.
- End Date - Year of Death

- ## 2. Artwork Table
    Includes data about each artwork in the collection :
- Object ID - Unique identifier for each artwork.
- Title - Title of the artwork.
- Constituent ID - Artist's ID.
- Date - Artwork creation Date.
- Medium - Materials used for the artwork.
- Dimensions - Size of the artwork.
- Classification - Size of the artwork.
- Department - MOMA department responsible for the artwork.
- Date Acquired - Artwork Acquisition Date.
- On View - Where the artwork is currently on display at the Museum.
- URL - Link to the artwork on MOMA's website.
- Image URL - Direct link to image of the artwork.
  The Csv file can be downloaded here.

# Tools and Technologies used 
1. Power BI : This was the major tool used for this project. Power BI was used to create interactive dashboards and visualization for the insights generated from this project.
2. Power Query Editor : The power query editor was used for data cleaning and transformation across different columns.

# Project Workflow
A project workflow provides structure for every data analytics projects . It keeps the project organized and aligned with goals .The workflow of this project are :
1. Project Objective
2. Data Collection
3. Data Cleaning and Preparation
4. Data Visualization
5. Interpretation & Reporting

# Project Objective
The objectives of this project was to analyze the Musuem of Modern Art On View (MOMA) collection to undercover patterns and insights that highlight the diversity, acquisition trends, and the visibility of artworks and artists. 

# Data Collection 
The data for this project was collected from Maven Analytics . The data included the Artworks and Artist records from the Museum in New York City.

# Data Cleaning and Preparation
The data cleaning process began in Power Query Editor in Power BI. The major operation includes

- ## Artist Table
- Changed Data Types for each columns: Constituent ID was changed to Number, Artist Name,ArtistBio, Nationality, Gender was changed to Text .
- Replaced Null Values in Nationality and Gender to Unknown
- Renamed DisplayName column to Artist Name for Clarity.
- Text Operation such as changing the alphabet case from lower case to Proper Case.
- Removed Unnecessary Columns. The M Query Codes from the Power Query Editor have been attached to this repository.

- ## Artwork Table
- Changed Data Types for column with incorrect data types.
- Created a new column for Year Extracted . Used a formula to extract the first 4 digits number from the Date column.
- Replaced Inconsistencies values in Year Extracted Column for accuracy. The M Query Codes from the Power Query Codes have been attached to this repository.

In Addition, i created new measures and new column to provide deeper insights into MOMA ON VIEW Analysis:
- Total Artworks : To calculate artworks on view in the museum.
- Total Artist : To calculate Artist with Artwork in the museum.
- Total Medium
- Most Featured Artsit : Artist with the Most Artwork
- Male Artist
- Female Artist
- Total Department
- Total Classification

Additional Transformation includes 
- Created new column to calculate each Artist First Artwork and Age at First Artwork.
- New column to group the Age at First Artwork.
- New column to calculate Artist Artwork Count
- Created New Column to calulate Acquisition Time Period.  A calendar Table was created to support Artwork Date Acquired.

# Data Model 
The Data Model was automatically created in Power BI. This shows the relationship between the various Table in this project.

# Data Analysis & Visualization
After the completion of data cleaning and preparation, i proceeded to begin my analysis and visualization. To ensure easy readability and understanding, i divided the visualization into 5 pages.
Some Key insights from the data visualization are summarized below:

# Overview
The MOMA Dashboard provides a comprehensive snapshot of the museum's artwork collection, revealing important patterns in artist representation, medium distribution, acquisition trends, and gender diversity among artists.
The Museum of Modern Art holds a total of 1,345 artworks created by 661 distinct artists. These works span across 481 unique mediums, illustrating the museum’s commitment to a wide variety of artistic forms and practices. The most featured artist in the collection is Robert Frank, with 55 artworks, making him the most represented individual.
The top five artists, Robert Frank leads with a significant number of pieces, followed by Henri Matisse, Pablo Picasso, Jacob Lawrence, and an unidentified photographer.
In terms of classification, the collection is heavily dominated by paintings, drawings, and photographs. Paintings alone account for 321 items, followed closely by drawings (260) and photographs (240). Other major classifications include design objects, sculptures, prints, and architectural works.
The acquisition trends show a sharp increase in the number of artworks acquired in recent years. Between 2011 and 2024, the museum acquired 497 pieces more than any other time period highlighting an active acquisition strategy in the past decade. This contrasts with lower acquisition numbers in earlier decades, particularly before 1950.
Gender representation among artists reveals male artist have the highest artworks. Out of 661 artists, 421 artworks are attributed to male artists, while only 191 are by female artists. Additionally, 40 artworks come from artists whose gender is unknown, and just one artwork is attributed to a transgender woman. 

# Artist
The Artists section of the MoMA Dashboard provides valuable insights into the gender distribution, nationality, and activity status of artists represented in the museum's collection. 
Artist nationalities reveals a strong American dominance. Out of the top five nationalities, American artists account shows a substantial 292 entries, The second most common nationality, French, which stands at 51. German, British, Italian, and Japanese artists all appear equally in the dataset, each with 22–30 artists represented. Additionally, 22 artists have an unknown nationality, indicating either limited biographical data or anonymous contributions.

The age/status distribution of the artists offers further context about their periods of activity. Most artists fall into the 20–35 and 36–55 age brackets, with 285 and 276 artists respectively. These two age ranges dominate the data, suggesting that the museum's acquisitions are largely focused on emerging and mid-career artists. A smaller number of artists are categorized in the 56–75 range (42 artists), while only 6 artists are recorded as 76 and upward. A considerable portion about 35 artists—have an "unknown" status, and  there were some uncertainities in ages that falls between (1–12 years) and a smaller group falls between 13–19 years.

The bottom of the dashboard includes a searchable artist table, listing names along with their nationality, gender, and total number of artworks in the collection. For example, American male artist Aaron Siskind has 10 artworks, while several other artists such as Agnes Martin and Abdel Kader El-Janabi are represented by only one.

![image](https://github.com/user-attachments/assets/b6eee6b0-c0a8-4996-a6c8-5a8a90eb0514)


# Artwork
The Artworks section of the MoMA Dashboard gives a detailed overview of how artworks in the collection are distributed across mediums, departments, and classifications. The data reveals that the collection encompasses 481 unique mediums, spread across 6 departments and categorized into 20 classifications. This diversity reflects MoMA’s wide-ranging curatorial scope and its embrace of both traditional and contemporary art forms.

Among the departments, Painting & Sculpture leads with 455 artworks, followed by Drawings & Prints with 404. These two departments alone account for the majority of the museum's holdings. Architecture & Design (235 artworks) and Photography (226) also represent significant portions of the collection. In contrast, Media and Performance (21 artworks) and Film (4 artworks) are minimally represented, suggesting more niche or emerging curatorial focus areas.

When examining medium usage, the top five most commonly used mediums show a strong preference for traditional techniques. Oil on canvas tops the list with 185 artworks, followed by gelatin silver print (158), and various forms of drawing media such as ink, colored ink, and crayon on paper (132). Bronze (31) and casein tempera on hardboard (30) round out the top five, showing a blend of sculptural and mixed media approaches.

The classification breakdown aligns closely with these observations. Painting is the most dominant classification, with 321 artworks, followed by drawing (260) and photograph (240). Other significant classifications include design (143), sculpture (125), and print (88). More specialized or less represented classifications such as architecture (67), video (16), installation (15), and illustrated books (9) show MoMA’s expanding interest in multimedia and non-traditional formats.

Overall, this section emphasizes MoMA's traditional strengths in painting, drawing, and photography, while also highlighting its efforts to diversify into other media and departments. The dominance of established mediums like oil on canvas and gelatin silver print indicates a strong foundation in classic techniques, even as newer forms such as performance and video remain areas for potential growth.

# Time Analysis
The Time Analysis section of the MoMA Dashboard provides a temporal breakdown of artwork acquisitions, offering insight into when works have entered the museum's collection. The data is categorized by weekday, month, and year range, helping identify key periods of curatorial activity.

Acquisition by Weekday
Artwork acquisition shows a clear preference for certain days of the week. Tuesday stands out as the most active day, with 455 artworks acquired, significantly more than any other day. It is followed by Wednesday with 270 artworks, and Thursday with 269. Monday also sees a notable number of acquisitions at 254. Conversely, Sunday (44), Friday (40), and especially Saturday (6) show much lower activity, suggesting that acquisitions are primarily processed on weekdays.

Acquisition by Month
When analyzing acquisition by month, October leads substantially with 394 artworks acquired, followed by May with 176. Other months with relatively high acquisition activity include December (131), November (113), and June (110). The remaining months—particularly January (94), September (84) , and February (78) reflect moderate activity. April (75),March (76), July (5),and August (2) represent the lowest acquisition periods, with August and July showing a near halt in acquisitions.

Acquisition by Year Range
To provide better historical context, acquisition years are grouped into six ranges. The 2011–2024 period accounts for the highest number of acquisitions, totaling 497 artworks, which reflects MoMA’s recent expansion and curatorial activity. The 1991–2010 period follows with 270 artworks, while 1951–1970 and before 1950 account for 217 and 184 respectively. The 1971–1990 range has 170 artworks. Only 7 artworks are tagged with unknown acquisition years, suggesting strong data integrity in this dimension.

# Map
The Map section of the MoMA Dashboard visually represents the geographical distribution of artist nationalities featured in the museum's collection. This interactive component allows users to understand the global reach of the MoMA collection by locating the countries associated with each artist’s nationality on a world map.

The data includes a diverse range of nationalities, spanning North and South America, Europe, Africa, Asia, and Oceania. Notable among these are large representations from American, British, French, German, and Italian artists—countries traditionally associated with strong modern and contemporary art movements. Other well-represented nationalities include Japanese, Dutch, Canadian, and Spanish.

The map also showcases artists from less commonly represented regions, underscoring MoMA’s growing inclusivity. These include nationalities such as Bangladeshi, Ethiopian, Mozambican, Native American, Oneida, Kuwaiti, Senegalese, and Trinidad and Tobagonian, among others. This illustrates a commitment to cultural diversity and a broadening of curatorial horizons beyond Western art centers.

Additionally, some entries are categorized under “Unknown”, which likely indicates either missing nationality data or artists whose origins could not be definitively identified.

# Conclusion
The MoMA Dashboard provides a powerful analytical lens into the Museum of Modern Art’s collection, revealing critical patterns in artist demographics, artwork mediums, acquisition timelines, and global representation. Through interactive visualizations and curated data views, the dashboard surfaces both strengths and disparities in the collection’s makeup empowering stakeholders to make informed, data-driven decisions.

The insights uncovered highlight areas of excellence, such as MoMA’s strong holdings in painting, photography, and mid-to-late 20th-century works. At the same time, they draw attention to gaps in gender representation, underrepresented regions, and limited diversity in medium and classification. The clear trends in acquisition timing also offer opportunities to streamline institutional workflows and improve planning.

By translating data into actionable strategies, this dashboard supports MoMA’s mission to remain a leader in modern and contemporary art. With sustained focus on equity, inclusion, and global engagement, the museum can continue to evolve its collection to reflect a richer, more diverse art historical narrative.

This documentation, alongside the dashboard itself, serves as a foundational tool for ongoing evaluation and strategic development—ensuring MoMA’s collection continues to inspire, educate, and represent the full spectrum of creative expression.

# Recommendation
## 1. Support More Women and Gender-Diverse Artists
Increase the number of artworks by women and gender-diverse artists through targeted acquisitions and curated projects. Actively identify and include artists who have historically been overlooked due to gender bias. Collaborate with experts and researchers to guide these efforts. The goal is to raise representation by at least 25% over the next five years.

## 2. Include More Art from Around the World
Expand the collection by acquiring artworks from underrepresented regions, including Africa, South America, Southeast Asia, and the Middle East. Allocate dedicated funding and resources to ensure a focused and sustained effort. Build relationships with artists, institutions, and curators from these areas. Aim to increase the share of non-Western nationalities in the collection by at least 30%.

## 3. Add Different Types of Art
Address the low representation of certain mediums such as video, installation, illustrated books, and digital art. Double the number of acquisitions in these categories in the upcoming acquisition cycle. Invest in curatorial support and infrastructure to properly care for and present emerging media. This approach helps ensure the collection reflects the diversity of contemporary art practices.

## 4. Make Artist Representation More Fair
Prevent overrepresentation by capping the number of new acquisitions per individual artist. Prioritize investment in first-time acquisitions and works by emerging artists. Improve the overall distribution of artists in the collection to promote a more balanced and inclusive portfolio. This helps diversify artistic voices and ensures wider representation.

## 5. Plan Acquisitions Throughout the Year
Review and adjust internal acquisition workflows to avoid seasonal or end-of-year clustering. Distribute acquisition activities evenly throughout the calendar year. Align scheduling with funding cycles to improve planning and resource use. This ensures smoother operations and more consistent curatorial decision-making.

## 6. Fill Gaps in History and Improve Information
Launch initiatives to address missing historical periods and underrepresented movements within the collection. Focus on acquiring works that provide broader historical and cultural context. Improve the completeness and accuracy of metadata for all works in the collection. This enhances both research value and public accessibility.

## 7. Use Data to Guide Decisions
Integrate simple, visual data tools and dashboards into acquisition planning and reviews. Use data to track progress on diversity, equity, and representation goals. Conduct regular assessments to support strategic and informed decision-making. A data-informed approach ensures transparency and alignment with long-term objectives.

## 8. Build Partnerships to Expand Reach
Establish partnerships with regional museums, cultural ministries, and art fairs, especially in underrepresented areas. Use these collaborations to discover new artists and support cross-cultural exchange. Shared initiatives can increase access to artworks and strengthen international networks. These partnerships support a more globally representative collection.



