# 4D Graph Template

### What
Jupyter Notebook to graph summarised data 4 dimensionally.<br>
Inspired by the [Bokeh Crossfilter Example](https://demo.bokehplots.com/apps/crossfilter).

### How
The template works best with the anaconda python distribution.<br>
To copy the exact environment used to create this, create a conda environment from the yml file in this repo. <br>
Click [here](https://conda.io/docs/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file) for a how-to.

### Getting Started

1. Once opened, enter the location of the the csv you'd like to visualise.

   ![Step 1](https://user-images.githubusercontent.com/40549299/43490991-b50f0c04-951a-11e8-885a-1b3409a881cc.png)

2. Select the discrete (non-numeric) variables. 

   ![Step 2](https://user-images.githubusercontent.com/40549299/43491048-f02f03fc-951a-11e8-9cc4-d94da50c0ea1.png)

3. Select preferred settings, e.g. variables, colour scheme, circle size etc.

   ![Step 3](https://user-images.githubusercontent.com/40549299/43491154-47ada732-951b-11e8-98a7-a28910abbf77.png)

4. To save a graph as a static png, click the Save button in the top-right of the figure.
   To select an individual data point, click the linked table or hover over the circle to see tooltip information.

   ![Step 4](https://user-images.githubusercontent.com/40549299/43491234-a24d0732-951b-11e8-998e-e84b60e363bd.png)

   ![Tooltip](https://user-images.githubusercontent.com/40549299/43491502-c713e1a2-951c-11e8-8561-4c9808191750.png)

### Tips

* Ensure each unique variable in the data is a column.
    *  This is especially important for time-series data.

### Backlog

- Add a **Binder** for this
- Add log scale option
- File import wizard
  - Not currently possible.
- Add 'none' as an option for default variables
- Refactor code to avoid the use of **global** scope, return tuple instead (good practice).
- Change to 1-based indexing for row number tooltip?
- Move as many widgets to Bokeh from iPython without making it clunky
- Add all columns to data table
- Change continuous to categorical data,
  - Dropdown linked with slider? This may make it too complicated.
