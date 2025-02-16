# Working in the Jupyter ecosystem

Jupyter is a large umbrella project that covers different open-source software offerings and tools, including Jupyter Notebook and JupyterLab which are web-based notebook authoring and editing applications.

Both Jupyter Notebook and Jupyter Lab, are web applications that allow you to create and share documents that contain live code, narrative text, equations, and visualizations. They support various programming languages, including Python.
Jupyter notebooks are widely used in data science, academic research, and machine learning. In particular, they are great for experimenting and sharing your work with Plotly.

This recipe aims to help you to make your first interactive visualization within the Jupyter environment.

## Getting ready

Make sure you have a Python distribution (preferably 3.10 or higher) in your operative system. You can download it from [its official website](https://www.python.org/downloads/).

In addition, you need to have either Jupyter Notebook or Jupyterlab installed. 

If you're using Dash version 2.11 or later, you can directly run Dash apps within Jupyter Notebooks without any additional libraries.

## How to do it

1. Create a new Jupyter Notebook
2. Import dash

```bash
import dash
```

3. Check your dash version to make sure that it is at least 2.11. You can do this  by printing the version as follows. If you have an older version, upgrade it.

```python
import dash
print(dash.__version__)
```

4. Create your first interactive chart using Plotly Express and render it within the notebook

```python
# Import the Express module from Plotly as px
import plotly.express as px

# Create your first figure with Plotly!
fig = px.line(x=[1, 2, 3, 4, 5], y=[4, 1, 3, 2, 5], title="Hello Plotly!")
# Show the figure
fig.show()
```

## There’s more

There are several ways to display your Dash applications within Jupyter:

- Inline mode (default): app.run_server() - This will display the app within the notebook output. It is perfect when working with small applications. It allows you to experiment freely without leaving your current window.
- External mode: app.run_server(jupyter_mode='external') - This will print a URL in the notebook output. Clicking the URL will open the app in a new browser tab. This is a more suitable option for large applications which require more space.
- Tab mode: app.run_server(jupyter_mode='tab') - This will automatically open the app in a new browser tab.
- JupyterLab mode (requires JupyterLab 3): app.run_server(jupyter_mode='jupyterlab') - This will display the app in a separate tab within JupyterLab.

See also [Jupyter Official website](https://jupyter.org/).
