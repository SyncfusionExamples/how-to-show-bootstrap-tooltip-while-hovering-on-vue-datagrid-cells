<template>
  <div id="app">
    <ejs-grid :dataSource="data" :allowPaging="true" >
          <e-columns>
            <e-column field='OrderID' headerText='Order ID' textAlign='Right' width=90></e-column>
            <e-column field='CustomerID' headerText='Customer ID' textAlign='Center' width=120 :template="'cTemplate'">
              <template v-slot:cTemplate={data}>
                  <div class="text-center">
                    <span
                  v-b-tooltip.hover
                  :title="data.CustomerID"
                  >{{data.CustomerID}}</span
                >
              </div>
            </template>
            </e-column>
            <e-column field='Freight' headerText='Freight' textAlign='Right' format='C2' width=90></e-column>
            <e-column field='OrderDate' headerText='Order Date' textAlign='Right' type='date' format="yMd" width=120></e-column>
          </e-columns>
        </ejs-grid>
  </div>
</template>
<script>
import Vue from 'vue';
import { GridPlugin, Page } from '@syncfusion/ej2-vue-grids';
import { BootstrapVue, IconsPlugin } from 'bootstrap-vue';
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'
import { data } from './datasource.js';

Vue.use(BootstrapVue)
// Optionally install the BootstrapVue icon components plugin
Vue.use(IconsPlugin)

Vue.use(GridPlugin);
export default {
  name: 'app',
  data () {
    return {
      data: data,
    }
  },
  provide: {
      grid: [Page]
  },
}
</script>
<style>
@import "../node_modules/@syncfusion/ej2-base/styles/material.css";
@import "../node_modules/@syncfusion/ej2-navigations/styles/material.css";
@import "../node_modules/@syncfusion/ej2-vue-grids/styles/material.css";
</style>