\# Social Network Recommendation System — Pure Python



A Python-based project that processes social-network data and generates simple recommendations using \*\*friend connections\*\* and \*\*shared interests\*\*.



This project is built using \*\*core Python and JSON data\*\*, without using Pandas or NumPy. The main focus is understanding data processing, data cleaning, and recommendation logic using Python's fundamental data structures.



\## Project Overview



The project works with structured social-network data containing:



\* Users

\* Friend connections

\* Liked pages

\* Page information



The project processes this data through multiple stages, from loading and cleaning the data to generating recommendations.



\## Features



\### 1. Social Network Data Processing



The project loads JSON data and works with user information, friend relationships, and liked pages.



\### 2. Data Cleaning



The project works with sample data containing issues such as:



\* Empty user names

\* Duplicate friend IDs

\* Duplicate page IDs

\* Users with no friends or liked pages



The data is cleaned before being used for further analysis.



\### 3. People You May Know



The project generates possible friend recommendations using \*\*mutual friends\*\*.



The basic process is:



```text

User

&#x20; ↓

Direct Friends

&#x20; ↓

Friends of Friends

&#x20; ↓

Find Mutual Friends

&#x20; ↓

Remove Existing Friends

&#x20; ↓

Count Mutual Connections

&#x20; ↓

Recommend People

```



\### 4. Pages You Might Like



The project also generates page recommendations using \*\*shared interests\*\*.



The basic process is:



```text

User's Liked Pages

&#x20;       ↓

Compare with Other Users

&#x20;       ↓

Find Shared Interests

&#x20;       ↓

Calculate Recommendation Score

&#x20;       ↓

Recommend Pages

```



\## Project Structure



```text

social-network-recommendation-system/

│

├── 01\_cfd.ipynb

├── 02\_cfd.ipynb

├── 03\_cdf\_you\_may\_know.ipynb

├── 04\_pages\_you\_might\_like.ipynb

│

├── data.json

├── data2.json

├── cleaned\_data2.json

├── massive\_data.json

│

├── .gitignore

└── README.md

```



\## File Description



| File                            | Purpose                                              |

| ------------------------------- | ---------------------------------------------------- |

| `01\_cfd.ipynb`                  | Works with the initial social-network data           |

| `02\_cfd.ipynb`                  | Works with data processing and cleaning              |

| `03\_cdf\_you\_may\_know.ipynb`     | Implements people-you-may-know recommendation logic  |

| `04\_pages\_you\_might\_like.ipynb` | Implements page recommendation logic                 |

| `data.json`                     | Initial sample dataset                               |

| `data2.json`                    | Sample dataset containing data-quality issues        |

| `cleaned\_data2.json`            | Cleaned version of the sample data                   |

| `massive\_data.json`             | Larger dataset for testing recommendation logic      |

| `.gitignore`                    | Prevents Jupyter checkpoint files from being tracked |



\## Python Concepts Used



This project uses fundamental Python concepts including:



\* Variables

\* Lists

\* Dictionaries

\* Sets

\* Loops

\* Functions

\* Conditional statements

\* List comprehensions

\* File handling

\* JSON

\* Sorting



\## Data Processing Concepts



The project demonstrates:



\* Loading JSON data

\* Traversing nested lists and dictionaries

\* Checking data types

\* Handling missing values

\* Removing duplicates

\* Cleaning structured data

\* Transforming data

\* Finding common elements using sets



\## Recommendation Logic



The recommendation system in this project is \*\*rule-based\*\*, not machine-learning based.



\### People Recommendation



Possible people are identified using relationships between users and their friends. Mutual connections are counted and used to determine recommendation scores.



\### Page Recommendation



Pages are compared based on users' liked pages. Shared interests are used to calculate recommendation scores.



\## Dataset



The project uses \*\*sample data created for learning and testing\*\*. It does not use real users or real social-network data.



The larger sample dataset contains multiple users, friendship relationships, and technology-related pages.



\## Purpose of the Project



The purpose of this project is to understand how social-network data can be processed and how basic recommendation logic can be developed using \*\*pure Python\*\*.



The project focuses on building programming and problem-solving skills before moving toward advanced data-science and machine-learning techniques.



\## Learning Outcomes



Through this project, I practiced:



\* Working with nested JSON data

\* Writing reusable functions

\* Traversing lists and dictionaries

\* Using sets for duplicate removal and common-element detection

\* Cleaning inconsistent data

\* Designing basic recommendation logic

\* Calculating recommendation scores

\* Sorting recommendation results



\## Technologies Used



\*\*Language:\*\* Python



\*\*Data Format:\*\* JSON



\*\*Environment:\*\* Jupyter Notebook



\*\*Libraries:\*\* Python standard library



\## Future Improvements



Possible future improvements include:



\* Improving recommendation scoring

\* Adding more recommendation criteria

\* Supporting larger datasets

\* Adding data visualization

\* Creating a user interface

\* Converting the project into a web application

\* Exploring machine-learning-based recommendation techniques



\## Note



This is a learning project focused on understanding \*\*Python data processing and basic recommendation-system logic\*\* using fundamental programming concepts.




