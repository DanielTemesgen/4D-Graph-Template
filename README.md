# 4D Graph Template

Jupyter Notebook to graph summarised data 4 dimensionally.

Originally inspired by the [Bokeh Crossfilter Example](https://demo.bokehplots.com/apps/crossfilter).

#### Format
* Ensure each unique variable in the data is a column.
    *  This is especially important for time-series data.

## Roadmap

### Backlog
*  Add easy style themes
   *  Automatic setting of other specific widgets
*  Add log scale option
*  File import wizard
   * Not currently possible.
*  Add 'none' as an option for default variables
*  Refactor code to avoid the use of **global** scope, return tuple instead (good practice).
*  Change to 1-based indexing for row number tooltip?
*  Move as many widgets to Bokeh from iPython without making it clunky
*  Add all columns to data table
*  Change continuous to categorical data,
   *  Dropdown linked with slider? This may make it too complicated.

### Pre GitHub Progress
*  **14/05/2018**
    *  Added hover line colour to line colour widget
*  **11/05/2018**
    *  Link in grid line colour to plot
*  **10/05/2018**
    *  Added hover colour widget
    *  Refactored layout dictionary to swap VBox and HBox around
    *  Change hover tooltips out of standard form
    *  Disable warnings.
*  **30/04/2018**
    *  Added widgets for text colour
    *  Changed default colours
    *  Changed default sizes.
*  **29/04/2018**
    *  Add helpful link to understand colour schemes.
    *  Add vertical box layouts from layout dictionary
    *  Replaced size qcut with sklearn mixmaxscaler, as the quartile approach proves inaccurate for data with a wide range.
    *  Added widgets for 
       *  font sizes
       *  size range
       *  number of colour categories
       *  reverse colour scheme checkbox
       *  number of colour categories
*  **27/04/2018**
    * Fix qcut issue
      *  Fixed by using 'duplicates = drop' as an optional argument
*  **26/04/2018**
    *  Added user-defined color scheme.
    *  Add chosen colour and size variables to the plot title
      *  To make it easier to see information upon save.
*  **25/04/2018**
    *  Laid out widgets more nicely.
    *  Added save tool.
*  **24/04/2018**
    *  Added custom error messages.
*  **19/04/2018**
    *  Added widgets for initial setup
    *  Formed functions for click journey
*  **16/04/2018**
    *  Added data table below the plot
    *  Linked hover, circle with row of data?
      *  Did this by adding a datatable function which could pick up changes in the ColumnDataSource, then referenced this in the update function.
    *  ColorBar to the right of the plot
*  **12/04/2018**
    *  User options
      *  Colour
      *  Plot size
      *  Colour
      *  Size
      *  Transparency
      *  Tooltips