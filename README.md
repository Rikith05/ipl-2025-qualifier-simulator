# IPL-2025-Qualifier-Simulator

🏏 IPL Qualification Simulator

This project is an interactive Streamlit application that simulates different qualification scenarios for IPL teams based on the current points table and remaining fixtures. It allows users to test both best-case automatic simulations and manual match outcomes to check if a team can qualify for the playoffs.

📖 Features

Interactive UI built with Streamlit https://streamlit.io
Load either a default Excel file or upload custom datasets.

Two simulation modes:

Forced Best-Case Scenario → Calculates whether a selected team can still qualify by optimizing match outcomes.

Manual Scenario → User selects winners for each remaining match.

Data cleaning to handle team names consistently.

Visualizations with Plotly https://plotly.com :

Points progression bar chart (before vs after simulation).

Rank progression line chart across matches.

Validation messages to confirm whether the selected team qualifies.

🛠️ Tech Stack

Python 3.9+

Streamlit for the web interface

Pandas for data manipulation

OR-Tools (Google) for optimization in best-case scenario simulations

Plotly Express for charts

re for regex-based team name cleaning

📂 Input Data

The app requires an Excel file with two sheets:

points table → Current IPL points standings (columns: Team, Wins, Losses, Points).

schedule → Remaining matches (columns: Team1, Team2).

By default, the app attempts to load IPL_2025_Points_Table.xlsx. Users can also upload custom files via the sidebar.

🚀 How to Run

Clone the repository:
git clone https://github.com/Rikith05/ipl-2025-qualifier-simulator.git

cd ipl-simulator

Install dependencies:
pip install -r requirements.txt

Start the Streamlit app:streamlit run app.py

Open your browser at [http://localhost:8501 ](http://localhost:8501/)

📊 Example Output

Final Points Table after simulations.

Bar Chart comparing team points before and after simulations.

Line Graph showing ranking progression across matches.

Match Outcome Log listing winners and losers per game.

📦 Requirements File (requirements.txt)

streamlit
pandas
plotly
ortools
openpyxl

✅ Future Enhancements

Support for net run rate (NRR) calculations.

Option to simulate multiple teams simultaneously.

Export results as PDF or Excel.
