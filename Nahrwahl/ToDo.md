# General

- IT nach JIRA Board fragen
# Backend

## Required Additions

### Diaries
- Database Collection & API Endpoints

### Users
- `/update` and `/profile` endpoints


# Frontend

## General

- Maybe design it with gamification in mind (Jane McGonigal - Besser als die Wirklichkeit!)
- TypeScript
- React
- Axios/Fetch
- Tailwind CSS
- 


---

# Optional Additions

## FoodItem Collection:
### Filtering
- Methods for filtering food items based on different nutritional criteria, such as calorie range, protein content, etc.

### Pagination
- Methods to handle pagination, especially if you expect the number of food items to be large.

### Relations
- If `FoodItem` objects can be related to other entities (like user accounts, for example), methods for handling those relations could be useful.

### Count
- A method to get the total count of food items, optionally with filters applied, could be useful for frontend pagination logic.

### Versioning
- If your data might change frequently, consider adding version control for `FoodItem` objects. This way, you can prevent update conflicts.

### Soft Delete
- Instead of actually removing the `FoodItem` from the database, mark it as deleted and filter it out in subsequent calls. This is useful for undo functionality or data auditing.


---

# User
- [ ] Add `/update` service method
- [ ] Add `/update` controller endpoint
	- [ ] Add `/login` functionality
	- [ ] Add `/logout` functionality
- [ ] Add `/update/{username}` functionality for admin only

