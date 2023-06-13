- 👋 Hi, I’m @dforrester7735
- 👀 I’m interested in ...
- 🌱 I’m currently learning.
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

I would love some help in solving this: 

After running this code I get the following message:

    dcc.Dropdown(
      ^
SyntaxError: invalid syntax

# Import required packages
import pandas as pd
import dash
import dash_core_components as dcc
import dash_html_components as html
import plotly.express as px
from dash.dependencies import Input, Output

# Add Dataframe

# Add a bar graph figure

app = dash.Dash()
app.layout = html.Div(children=[
    html.H1(
        children='Dashboard',
        style={
            'textAlign': 'center'
        }
    )
       
    # Create dropdown
   dcc.Dropdown(
        options=[
            {'label': 'New York City', 'value': 'NYC'},
            {'label': 'Montréal', 'value': 'MTL'},
            {'label': 'San Francisco', 'value': 'SF'}
        ],
        value='NYC' # Providing a value to dropdown
    )

    # Bar graph
])

# Run Application
if __name__ == '__main__':
    app.run_server()


<!---
dforrester7735/dforrester7735 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
