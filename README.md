Visualizing the Most-Starred Python Projects on GitHub

This script retrieves data from the GitHub API to analyze and visualize the most-starred Python projects.

Using Plotly, the script generates an interactive bar chart displaying repositories, their star counts, and additional details like the owner's username and project description.

How It Works
1. API Call:
-The script uses the GitHub API to search for Python repositories, sorted by the number of stars.
-The requests library is used to send an API request, and the response is processed as JSON.

2. Data Processing:
-Extracts repository  names, URLs, star counts, and descriptions.
-Formats repository names as clickable links for the visualization.

3. Visualization:
-Creates an interactive bar chart using Plotly.
-Displays repository names on the x-axis, star counts on the y-axis, and hover text with additional details.

Features
-Interactive Visualization:
  - Hover over a bar to see the repository owner and description.
  - Click on a bar to navigate to the repository on GitHub.

-Custom Styling:
  - Bars are styled with a blue gradient and subtle outlines for clarity.
  - Chart title and axis labels are professionally formatted.

-Dynamic Data:
  - Fetches the latest repository data, ensuring up-to-date results.


Requirements
Python 3.6 or later
Required Python libraries:
-requests
-plotly
Install the dependencies using:
    - pip install requests plotly

How to Run
1. Clone the repository or copy the script.
2. Install the required Python libraries.
3. Run the script:
    - python most_starred_python_projects.py
4. Open the generated python_repos.html file in a web browser to view the visualization.

Customization
-To fetch repositories for a different programming language, modify the language parameter in the URL:
   - url = 'https://api.github.com/search/repositories?q=language:javascript&sort=stars'
-Adjust chart colors, opacity, and other visualization settings in the marker and layout dictionaries.
