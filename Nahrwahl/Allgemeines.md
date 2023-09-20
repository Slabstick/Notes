## Projektstruktur

```
Nahrwahl/
|-- src/
|   |-- main/
|       |-- java/
|           |-- com/
|               |-- yourcompany/
|                   |-- Nahrwahl/
|                       |-- config/           // Configuration classes
|                       |-- controller/       // REST controllers
|                       |-- model/            // Data models
|                       |-- repository/       // Data access layer
|                       |-- service/          // Business logic
|                       |-- NahrwahlApplication.java  // Main class
|       |-- resources/
|           |-- application.properties       // Spring Boot config
|-- build.gradle                              // Gradle build file


```

## Datenbank Outline

## Collections Overview

1. **Users Collection**: To store user-related data like username, email, etc.
2. **Food Items Collection**: To maintain a catalog of food items that users can add to their daily diets.
3. **Daily Diets Collection**: To keep track of what each user eats each day, including the portion sizes.

### Detailed Schema

#### 1. Users Collection

Stores basic user information.

```json
{
  "_id": ObjectId("uniqueUserID"),
  "username": "john_doe",
  "email": "john@example.com",
  // additional fields
}

```

#### 2. Food Items Collection

A catalog of food items with details such as caloric content per unit weight.

```json
{
  "_id": ObjectId("uniqueFoodItemID"),
  "user_id": ObjectId("uniqueUserID"), // Reference to user who added the food item
  "name": "Apple",
  "calories_per_100g": 52,
  // additional fields like macros, brand, etc.
}

```
#### 3. Daily Diets Collection

Stores the daily food intake for each user, including the portion sizes for each food item.

```json
{
  "_id": ObjectId("uniqueDailyDietID"),
  "user_id": ObjectId("uniqueUserID"), // Reference to the user
  "date": ISODate("2023-09-20"),
  "foods_consumed": [
    {
      "food_item_id": ObjectId("uniqueFoodItemID"), // Reference to food item
      "portion_size_g": 150,
      // additional fields
    },
    // More food items consumed
  ]
}

```
## Considerations

1. **References**: The `user_id` and `food_item_id` act as references linking the collections.
    
2. **Data Integrity**: These references help maintain data integrity and allow for cross-collection queries.
    
3. **Indexing**: You might also want to consider creating indexes on frequently queried fields to speed up data retrieval.
    
4. **Additional Collections**: Depending on further requirements, you might add more collections for features like exercise tracking, user preferences, or saved meals.