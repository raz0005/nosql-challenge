# UK Food Hygiene Ratings Analysis

## Overview

This repository contains a Jupyter notebook for analyzing the UK Food Standards Agency’s food hygiene ratings data. The analysis focuses on exploring, updating, and evaluating various aspects of the food hygiene ratings for establishments across the UK using MongoDB.

## Contents

- [`uk_food_analysis.ipynb`](uk_food_analysis.ipynb): Jupyter notebook containing all the steps for database setup, data updates, and exploratory analysis.
- [`establishments.json`](establishments.json): The JSON file with the food hygiene ratings data (if included; otherwise, this file can be downloaded from the source).
- [`README.md`](README.md): This file, providing an overview and instructions.
Certainly! Here's the README content formatted for GitHub. You can copy and paste this directly into your `README.md` file on GitHub.

```markdown
# UK Food Hygiene Ratings Analysis

## Overview

This repository contains a Jupyter notebook for analyzing the UK Food Standards Agency’s food hygiene ratings data. The analysis focuses on exploring, updating, and evaluating various aspects of the food hygiene ratings for establishments across the UK using MongoDB.

## Contents

- [`uk_food_analysis.ipynb`](uk_food_analysis.ipynb): Jupyter notebook containing all the steps for database setup, data updates, and exploratory analysis.
- [`establishments.json`](establishments.json): The JSON file with the food hygiene ratings data (if included; otherwise, this file can be downloaded from the source).
- [`README.md`](README.md): This file, providing an overview and instructions.

### Importing the Data

1. **Start MongoDB**: Ensure your MongoDB server is running.
2. **Import the Data**: Use the following command to import the `establishments.json` file into MongoDB:

    ```bash
    mongoimport --drop --db uk_food --collection establishments --file establishments.json
    ```

### Running the Jupyter Notebook

1. **Start Jupyter Notebook**:

    ```bash
    jupyter notebook
    ```

2. **Open the Notebook**: Navigate to the `uk_food_analysis.ipynb` file in the Jupyter interface and open it.

3. **Run the Cells**: Follow the instructions in the notebook to execute each cell. The notebook includes sections for database setup, data updates, and exploratory analysis.

## Part 1: Database and Jupyter Notebook Set Up

This section of the notebook sets up the MongoDB connection, imports the data, and verifies the setup.

### Key Steps:
- Import `establishments.json` into the `uk_food` database.
- Connect to MongoDB and list databases and collections.
- Display a sample document from the `establishments` collection.

## Part 2: Update the Database

This part includes tasks to update the database with new information and modify existing data.

### Key Tasks:
- Insert a new document for "Penang Flavours."
- Find and update the `BusinessTypeID` for "Restaurant/Cafe/Canteen."
- Remove documents with `LocalAuthorityName` as "Dover Local Authority."
- Convert `Latitude`, `Longitude`, and `RatingValue` fields to appropriate data types.

## Part 3: Exploratory Analysis

This section involves querying and analyzing the data to answer specific questions.

### Key Questions:
1. **Hygiene Score of 20**: Find establishments with a hygiene score of 20.
2. **London Establishments with RatingValue >= 4**: Identify establishments in London with a rating value of 4 or higher.
3. **Top 5 Establishments Near "Penang Flavours"**: List the top 5 establishments with a rating value of 5, closest to "Penang Flavours," sorted by the lowest hygiene score.
4. **Hygiene Score of 0 by Local Authority**: Aggregate and list the number of establishments with a hygiene score of 0 by local authority, sorted from highest to lowest.

## Deployment and Submission

### GitHub Repository

- Ensure you have committed and pushed your notebook and related files to your GitHub repository.
- Provide a link to your GitHub repository for submission.

### Example Commands:

```bash
git init
git add uk_food_analysis.ipynb
git commit -m "Add Jupyter notebook for UK food hygiene ratings analysis"
git branch -M main
git remote add origin <your_repository_url>
git push -u origin main
```

## Comments

The Jupyter notebook includes comments and explanations to ensure clarity and help reviewers understand the process and logic used throughout the analysis.

## Contact

For any questions or further clarifications, please contact [Your Name] at [Your Email].
```

Replace `<your_repository_url>`, `[Your Name]`, and `[Your Email]` with the appropriate information for your repository and contact details.
