# Render Bootstrap Tooltip in Grid Cells

## Repository Description

This repository contains a Vue.js sample that demonstrates how to render Bootstrap tooltips inside Syncfusion Vue DataGrid cells by integrating BootstrapVue with custom column templates.

## Project Overview

This sample illustrates how to enhance the user experience of a Syncfusion Vue DataGrid by displaying Bootstrap tooltips within grid cells. Tooltips are useful when cell content needs additional context or when values are truncated due to limited column width. In this implementation, Bootstrap tooltip directives are applied inside a column template to display tooltip text when users hover over specific cell values.

The project is built using Vue 2 and integrates Bootstrap, BootstrapVue, and the Syncfusion Vue Grid component. By combining these libraries, the sample shows how third-party UI utilities such as Bootstrap tooltips can work seamlessly with Syncfusion grid features like paging and data binding.

## Key Features

- Syncfusion Vue DataGrid integration
- Bootstrap and BootstrapVue tooltip support
- Custom column templates for grid cells
- Hover-based tooltip rendering inside grid columns

## Prerequisites

- Node.js and npm
- Basic knowledge of Vue.js

## Running the Application

Follow the steps below to install dependencies, run the application, and build it for production.

1. Clone the repository and navigate to the project directory:

   ```bash
   git clone https://github.com/SyncfusionExamples/how-to-show-bootstrap-tooltip-while-hovering-on-vue-datagrid-cells.git
   cd how-to-show-bootstrap-tooltip-while-hovering-on-vue-datagrid-cells
   ```

2. Install the required npm packages:

   ```bash
   npm install
   ```

   This installs Vue, Bootstrap, BootstrapVue, and the Syncfusion Vue Grid packages required for the application.

3. Run the application in development mode:

   ```bash
   npm run serve
   ```

   Once the development server starts, open the displayed local URL in a browser. Hover over the grid cell values to see Bootstrap tooltips rendered inside the DataGrid.

4. Build the application for production:

   ```bash
   npm run build
   ```

   This command compiles and minifies the application for deployment.

## Additional Resources

- [Syncfusion Vue Grid Documentation](https://ej2.syncfusion.com/vue/documentation/grid/getting-started)
- [Syncfusion Vue Grid Column Templates Documentation](https://ej2.syncfusion.com/vue/documentation/grid/columns/column-template)
- [BootstrapVue Tooltip Documentation](https://bootstrap-vue.org/docs/components/tooltip)
