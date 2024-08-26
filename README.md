

# Trip Planner Crew



## Overview

**Trip Planner Crew** is an application designed to help users plan their travel itineraries with the assistance of virtual agents. This project leverages CrewAI to automate the process of creating a detailed travel plan, including city selection, itinerary development, and local insights.

## What is CrewAI?

**CrewAI** is a platform that enables the creation of virtual teams composed of specialized agents and tasks. These agents are designed to perform specific roles and tasks, guided by clearly defined goals. CrewAI uses a top-down approach where you define a "captain" to lead and delegate tasks to other agents. The agents use various tools and resources to achieve the desired outcomes, which are then coordinated and managed by CrewAI.

## How It Works

1. **Agents and Tasks Definition**: Define the agents and tasks required for your project. Agents are specialized roles with specific expertise, while tasks outline the actions needed to achieve the project's goals.

## Project Explanation

In this project, the goal is to create a 7-day travel itinerary. The process involves:

1. **City Selection**: Analyzing and selecting the best cities to visit based on weather, season, prices, and traveler interests.

2. **Itinerary Planning**: Developing a detailed daily plan for the trip, including places to visit, budget, packing suggestions, and safety tips.

3. **Local Insights**: Gathering in-depth information about the selected cities, including attractions, local customs, and events.

The project uses three main agents:

- **Expert Travel Agent**: Responsible for creating a detailed 7-day itinerary.
- **City Selection Expert**: Helps in selecting the best city based on various criteria.
- **Local Tour Guide**: Provides insights and recommendations for the selected city.

## How to Run the Project

1. **Setup Environment**:
   - Ensure you have Python 3.x installed.
   - Install the required packages using pip:
     ```bash
     pip install crewai langchain_google_genai python-dotenv
     ```

2. **Configure Environment Variables**:
   - Create a `.env` file in the project directory.
   - Add your Google API key:
     ```env
     GOOGLE_API_KEY=your_google_api_key_here
     SERPER_API_KEY=your_serper_api_key_here
     ```
   
3. **Run the Project**:
   - Execute the `main.py` script:
     ```bash
     python main.py
     ```

4. **Input Details**:
   - Follow the prompts to enter your origin, cities of interest, date range, and interests.

5. **View Results**:
   - The application will print the generated trip plan, including detailed itinerary and city information.

## Example

```bash
## Welcome to Trip Planner Crew
-------------------------------
From where will you be traveling from?
[Your Origin]

What are the cities options you are interested in visiting?
[City List]

What is the date range you are interested in traveling?
[Date Range]

What are some of your high-level interests and hobbies?
[Your Interests]

## Here is your Trip Plan
...
```

## Notes

- Ensure your `.env` file is correctly configured with the necessary API keys.
- Customize the agents and tasks as needed for specific travel requirements.

For more information on CrewAI, refer to the [CrewAI Documentation](https://docs.crewai.com/).

---

