# Reproducibility Demo – CSC 786
## Food Waste Nutrition Analysis

This repository demonstrates an ethical, reproducible data-collection workflow used in the CSC 786 course.

## Overview
This project collects nutritional data from the USDA FoodData Central API to analyze the nutritional value of commonly wasted restaurant foods. By
documenting the caloric and macronutrient content of frequently discarded foods, this analysis highlights the environmental and nutritional impact of
food waste.

### Data Source
- **API**: USDA FoodData Central API
- **Endpoint**: `/foods/search`
- **Purpose**: Retrieve nutritional information for commonly wasted restaurant foods
- **Foods Analyzed**: French fries, bread, pizza, salad, chicken wings

### Research Question
What is the nutritional value (calories, protein, fats, carbohydrates) lost when commonly wasted restaurant foods are discarded?

## Files
| File | Purpose |
|------|----------|
| `README.md` | Project overview and usage instructions |
| `ETHICS.md` | Ethical statement for transparency |
| `DATA_README.md` | Auto-logged metadata for every data collection event |
| `data/` | Directory containing collected CSV files and visualizations |

## Visualizations
- `food_waste_calories_*.png` - Bar chart showing calorie content of commonly wasted foods
- `food_waste_nutrients_*.png` - Multi-nutrient comparison (protein, fat, carbohydrates)

## Requirements
- Python 3.x
- Libraries: pandas, requests, matplotlib, hashlib

## Usage
1. Obtain a free API key from https://fdc.nal.usda.gov/api-key-signup.html
2. Set the API key as an environment variable
3. Run the notebook to collect data and generate visualizations
4. All data collection events are automatically logged with provenance metadata

---
**Note**: This project complies with USDA FoodData Central API terms of service and rate limits.
