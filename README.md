# Test Scenario: Dating Analysis

### Background:
You work for a dating app company. Your goal is to analyze user behavior, preferences, and engagement patterns to provide insights into matching efficiency and user satisfaction.

Instructions:

1. Connect the data: Examine the datasets provided, identify relationships, and clean/transform the data as needed.
2. Analyze and extract insights: Generate new metrics to better understand user engagement and preferences.
3. Visualize the insights: Use Tableau (or your tool of choice) to create a dashboard showing meaningful insights. (can also be theoretical and explain how you would create it)

## Datasets (100 Rows Each)

<strong style="color: orange;">Please see the csv folder for the files</strong>

## Table examples and layout

### User Data

| UserID | Name          | Age  | Gender | Location       | Interests       | PremiumUser | SwipesLeft | SwipesRight |
|--------|---------------|------|--------|----------------|-----------------|-------------|------------|-------------|
| 1      | Alex Johnson  | 25   | Male   | New York       | Movies, Hiking  | Yes         | 120        | 80          |
| 2      | Sara Smith    | 30   | Female | Los Angeles    | Cooking, Travel | No          | 100        | 50          |
| ...    | ...           | ...  | ...    | ...            | ...             | ...         | ...        | ...         |

### Match Data
| MatchID | UserID1 | UserID2 | MatchDate   | MatchedOn     | MessagesExchanged | DateScheduled |
|---------|---------|---------|-------------|---------------|-------------------|---------------|
| 1       | 1       | 3       | 2024-01-10 | Hiking        | 10                | 2024-01-15    |
| 2       | 2       | 4       | 2024-01-12 | Travel        | 15                | 2024-01-20    |
| ...     | ...     | ...     | ...         | ...           | ...               | ...           |

### Geohraphical Data
| LocationID | City           | Region      | AvgAge | AvgIncome | ActiveUsers |
|------------|----------------|-------------|--------|-----------|-------------|
| 1          | New York       | Northeast   | 27     | 75000     | 1200        |
| 2          | Los Angeles    | West Coast  | 29     | 85000     | 900         |
| ...        | ...            | ...         | ...    | ...       | ...         |

### Subscription Data
| SubscriptionID | UserID | StartDate   | EndDate     | PlanType  | MonthlyCost |
|----------------|--------|-------------|-------------|-----------|-------------|
| 1              | 1      | 2024-01-01 | 2024-12-31  | Premium   | 20          |
| 2              | 3      | 2024-02-01 | 2024-05-01  | Standard  | 10          |
| ...            | ...    | ...         | ...         | ...       | ...         |

### Survey Data
| UserID | SatisfactionScore | Feedback                                              | RecommendToFriend |
|--------|-------------------|-------------------------------------------------------|-------------------|
| 1      | 8                 | Matches are relevant, premium worth it               | Yes               |
| 2      | 6                 | Too few matches in my area                           | No                |
| ...    | ...               | ...                                                   | ...               |

## Task
### 1. Data Cleaning & Transformation
- Identify and resolve missing or inconsistent data.
- Combine datasets (e.g., join matches with users and subscription data).
- Generate derived metrics like `EngagementRate = SwipesRight / (SwipesRight + SwipesLeft)`.
### 2. Analysis Questions
- What is the average engagement rate for each location?
- Which user demographic (age, gender, or location) is most likely to subscribe?
- What are the top three interests leading to matches?
- How does satisfaction score correlate with premium subscription?
### 3. Dashboard Requirements
- Visualize user engagement by location and demographic.
- Show satisfaction levels segmented by subscription type.
- Highlight key interests driving matches.
