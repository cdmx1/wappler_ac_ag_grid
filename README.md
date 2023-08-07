﻿Maintained by: Roney Dsilva
# AG Grid Module Documentation

The AG Grid module allows you to create a flexible and customizable data grid with various options and properties. Below, you'll find the list of properties and options available for configuring the AG Grid module:

## AG Grid Properties

1. **ID**: Unique ID for the grid. (Required)
2. **Data Source**: Data source for the grid. Enter the data source to populate the grid. (Required)
3. **No Auto Load**: Set to true to disable auto-load of the grid. (Default: true)
4. **Theme**: Select a theme for the grid.
   - "Alpine"
   - "Balham"
   - "Material"
   - "Base" (Default)
5. **Locale**: Select the locale for the grid. Currently supported locales: English (EN) and Hebrew (HE). (Default: EN)

## AG Grid Options
6. **Minimum Width**: The minimum width of the column. (Default: 150)
7. **Resizable**: Specifies if the column can be resized. (Default: true)
8. **Sortable**: Specifies if the columns are sortable. (Default: true)
9. **Filter**: Specifies if the column has a filter. (Default: true)
10. **Floating Filter**: Specifies if the column has a floating filter. (Default: true)
11. **CSV Export**: Specifies if Export to CSV is enabled. (Default: true)
12. **Enable RTL**: Enabled Right to Left, used for Hebrew and Arabic. (Default: false)
13. **Column Hover Highlight**: Specifies column hover highlighting. (Default: true)
14. **Suppress Row Deselection**: Specifies if rows can be deselected. (Default: false)
15. **Pagination**: Enables pagination. (Default: true)
16. **Pagination Page Size**: Number of rows to show per page. (Default: 20)
17. **Row Selection**: Row Selection (single or multiple).
   - "Single"
   - "Multiple" (Default)
18. **Timezone**: Timezone for Date Fields. Select the appropriate timezone from the dropdown list.
19. **Date Format**: Date Format for displaying date values. (Default: "dd/MM/yyyy hh:mm A")
20. **Sticky Header**: Enable sticky header. Optionally specify the header offset and topbar class.
   - Header Offset: Specifies offset from the top of the viewport area (Optional). (Default: 100)
   - Topbar Class: Specify class, e.g., "topbar", to measure the offset from (Optional). (Default: "topbar")
   - Topbar Offset: Specify topbar offset (Default: 80)
21. **Row Height**: Height of each row in pixels. (Default: 25)
22. **Header Height**: Height of the header row in pixels. (Default: 30)
23. **Suppress Row Click Selection**: Disables row selection on row click. (Default: false)
24. **Suppress Menu Hide**: Prevents hiding the column menu. (Default: false)
25. **Suppress Movable Columns**: Disables moving columns. (Default: false)
26. **Enable Cell Expressions**: Enables expressions in cell values. (Default: false)
27. **Animate Rows**: Enables row animation on data changes. (Default: false)
28. **Suppress Aggregation Function in Header**: Hides the aggregation function in column headers. (Default: false)
29. **Suppress Aggregation at Root Level**: Disables aggregation at the root level. (Default: false)
30. **Suppress Clipboard Paste**: Disables pasting data from the clipboard. (Default: false)
31. **Suppress Scroll on New Data**: Prevents scrolling to newly added data. (Default: false)
32. **Suppress Property Names Check**: Disables checking for duplicate property names. (Default: false)
33. **Hide ID Field**: Hides the ID Field in the Grid. (Default: false)
34. **Row Click Events**: Enables row click events. This can be used in Dynamic events => Grid Events => Row Clicked. (Default: false)
35. **Enable Row Selection**: Enables row selection. This can be used in Dynamic events => Grid Events => Checkbox Checked || Checkbox Unchecked. (Default: false)
36. **Enable Row Status Toggle**: Enables row status toggle events. This can be used in Dynamic events => Grid Events => Checkbox Checked || Checkbox Unchecked. (Default: false)

# Data Type Overrides

The Data Type Overrides feature allows you to configure type overrides for specific attributes in the data. This allows you to override the auto-detected data types.
This grid allows you to define custom type overrides for specific fields in the data. The grid has the following columns:

1. **Field**: The field name for which you want to override the data type. (Editable: text)
2. **Type**: The new data type you want to assign to the field. Choose from "number," "text," or "date." (Editable: list)

---

# Style Formatting

The Style Formatting feature allows you to configure custom colors and fonts for column data based on certain conditions.
This grid allows you to define custom color and font settings based on specific conditions. The grid has the following columns:

1. **Field**: The field name for which you want to apply the custom color and font settings. (Editable: text)
2. **Condition**: The condition to check for applying the custom color and font settings. (Editable: text)
3. **Color**: The custom color to apply when the condition is met. Enter the color in HEX format (e.g., "#FF0000") or use named colors (e.g., "red"). (Editable: text)
4. **Area**: Choose where to apply the color: "text" (cell text) or "cell" (cell background). (Editable: list)
5. **Font**: Choose the font style: "normal," "italic," or "bold." (Editable: list)
---

# Tooltip Settings

The Tooltip Settings feature allows you to configure custom tooltips for specific fields in the data.

To set a custom tooltip text, enter the desired text for the tooltip in the field.
This grid allows you to configure custom tooltips for specific fields. The grid has the following columns:

1. **Field**: The field name for which you want to set a custom tooltip. (Editable: text)
2. **Tooltip**: Choose whether to enable ("yes") or disable ("no") the tooltip for the field. (Editable: list)
---

# Advanced Data Manipulation

The Advanced Data Manipulation feature allows you to add custom values to the field data based on specific conditions.
This grid allows you to define custom data changes for specific fields. The grid has the following columns:

1. **Field**: The field name for which you want to apply the custom data changes. (Editable: text)
2. **Data**: The new data source or value to be used for the field. (Editable: date picker)
3. **Property**: The property within the data source to use as the new value for the field. (Editable: text)
4. **Output**: The output value for the field. (Editable: text)
5. **Area**: Choose where to apply the data changes: "cell" (cell text) or "tooltip" (tooltip text). (Editable: list)


---

# Data Manipulation

The Data Manipulation feature allows you to add custom values to the field data based on specific conditions.
This grid allows you to define custom data changes for specific fields. The grid has the following columns:

1. **Field**: The field name for which you want to apply the custom data changes. (Editable: text)
2. **Value**: The value to be replaced in the field data. (Editable: text)
3. **New Value**: The new value to replace the original value in the field data. (Editable: text)
4. **Area**: Choose where to apply the data changes: "cell" (cell text) or "tooltip" (tooltip text). (Editable: list)

---
**Configure Header Names**
This grid allows you to define custom header names for specific columns. The grid has the following columns:

1. **Field**: The field name for which you want to set a custom header name. (Editable: text)
2. **Name**: The custom header name to be displayed for the column. (Editable: date picker)

Please note that these changes will only take effect when the `cnames` attribute is set to `true`.

---

# Custom Widths

The Custom Widths feature allows you to configure custom column widths for columns.

**Configure Custom Widths**
This grid allows you to define custom column widths for specific columns. The grid has the following columns:

1. **Field**: The field name for which you want to set a custom column width. (Editable: text)
2. **Min Width**: The minimum width for the column. (Editable: text)
3. **Max Width**: The maximum width for the column. (Editable: text)

# Hide Fields and Filters

The Hide Fields and Filters feature allows you to hide components such as filters and fields.

**Hide Components**
This will display the "Hide Fields," "Hide Filters," and "Hide Sort Filters" fields with options to specify which components to hide.

**Hide Fields**
Enter the names of fields you want to hide separated by commas. The specified fields will be hidden from the view.

**Hide Filters**
Enter the names of filters you want to hide separated by commas. The specified filters will be hidden from the view.

**Hide Sort Filters**
Enter the names of sort filters you want to hide separated by commas. The specified sort filters will be hidden from the view.

---

# Configure Actions Column
The Configure Actions Column feature allows you to configure actions for the buttons in the Actions Column.

**Enable Actions**
This will display the "Configure Actions" options for the buttons in the Actions Column.

**Pin Actions Column**
This will keep the Actions Column fixed when scrolling horizontally.

**Edit Action Button**
This will display the "Edit Action Button" options.

**Edit Action Button Title**
Specify the title for the Edit Action button.

**Edit Action Button Tooltip**
Specify the tooltip text for the Edit Action button.

**Edit Action Button Class**
Specify the CSS class for styling the Edit Action button.

**Edit Action Icon Class**
Specify the CSS class for styling the icon of the Edit Action button.

**View Action Button**
This will display the "View Action Button" options.

**View Action Button Title**
Specify the title for the View Action button.

**View Action Button Tooltip**
Specify the tooltip text for the View Action button.

**View Action Button Class**
Specify the CSS class for styling the View Action button.

**View Action Icon Class**
Specify the CSS class for styling the icon of the View Action button.

**Delete Action Button**
**Delete Action Button Title**
Specify the title for the Delete Action button.

**Delete Action Button Tooltip**
Specify the tooltip text for the Delete Action button.

**Delete Action Button Class**
Specify the CSS class for styling the Delete Action button.
Specify the CSS class for styling the icon of the Delete Action button.

## License

The AG Grid module is licensed under the MIT License. Please refer to the license file for more details.

For any issues or further assistance, please contact our support team.

