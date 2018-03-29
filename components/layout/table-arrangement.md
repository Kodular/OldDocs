# Table Arrangement

Use a table arrangement component to display a group of components in a tabular fashion.

This component is a formatting element in which you place components that should be displayed in tabular form.

In a TableArrangement, components are arranged in a grid of rows and columns, with not more than one component visible in each cell. If multiple components occupy the same cell, only the last one will be visible.

Within each row, components are vertically center-aligned.

The width of a column is determined by the widest component in that column. When calculating column width, the automatic width is used for components whose Width property is set to Fill Parent. However, each component will always fill the full width of the column that it occupies.

The height of a row is determined by the tallest component in that row whose Height property is not set to Fill Parent. If a row contains only components whose Height properties are set to Fill Parent, the height of the row is calculated using the automatic heights of the components.

## Properties

### Visible

If true, component and its contents are visible.

### Rows \(number-of-rows\)

The number of rows in the table.

### Columns \(number-of-columns\)

The number of columns in the table.

### Height

Table arrangement height \(y-size\).

### Width

Table arrangement width \(x-size\).

