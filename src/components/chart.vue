<script>
import Vue from "vue";
import "@carbon/charts/styles.css";
import chartsVue from "@carbon/charts-vue";

// IBM Plex should either be imported in your project by using Carbon
// or consumed manually through an import
import "../ibm-plex-font.css";

Vue.use(chartsVue);

export default {
	name: "Chart",
	components: {},
	data() {
		return {
			data: [
		{
				"group": "Dataset 1",
				"date": "2018-12-31T16:00:00.000Z",
				"value": 10000
		},
		{
				"group": "Dataset 1",
				"date": "2019-01-04T16:00:00.000Z",
				"value": 65000
		},
		{
				"group": "Dataset 1",
				"date": "2019-01-07T16:00:00.000Z",
				"value": 10000
		},
		{
				"group": "Dataset 1",
				"date": "2019-01-12T16:00:00.000Z",
				"value": 49213
		},
		{
				"group": "Dataset 1",
				"date": "2019-01-16T16:00:00.000Z",
				"value": 51213
		},
		{
				"group": "Dataset 2",
				"date": "2019-01-02T16:00:00.000Z",
				"value": 75000
		},
		{
				"group": "Dataset 2",
				"date": "2019-01-05T16:00:00.000Z",
				"value": 57312
		},
		{
				"group": "Dataset 2",
				"date": "2019-01-07T16:00:00.000Z",
				"value": 21432
		},
		{
				"group": "Dataset 2",
				"date": "2019-01-14T16:00:00.000Z",
				"value": 70323
		},
		{
				"group": "Dataset 2",
				"date": "2019-01-18T16:00:00.000Z",
				"value": 21300
		},
		{
				"group": "Dataset 3",
				"date": "2018-12-31T16:00:00.000Z",
				"value": 50000
		},
		{
				"group": "Dataset 3",
				"date": "2019-01-04T16:00:00.000Z",
				"value": 15000
		},
		{
				"group": "Dataset 3",
				"date": "2019-01-07T16:00:00.000Z",
				"value": 20000
		},
		{
				"group": "Dataset 3",
				"date": "2019-01-12T16:00:00.000Z",
				"value": 39213
		},
		{
				"group": "Dataset 3",
				"date": "2019-01-16T16:00:00.000Z",
				"value": 61213
		},
		{
				"group": "Dataset 4",
				"date": "2019-01-01T16:00:00.000Z",
				"value": 10
		},
		{
				"group": "Dataset 4",
				"date": "2019-01-05T16:00:00.000Z",
				"value": 37312
		},
		{
				"group": "Dataset 4",
				"date": "2019-01-07T16:00:00.000Z",
				"value": 51432
		},
		{
				"group": "Dataset 4",
				"date": "2019-01-14T16:00:00.000Z",
				"value": 40323
		},
		{
				"group": "Dataset 4",
				"date": "2019-01-18T16:00:00.000Z",
				"value": 31300
		}
],
			options: {
		"title": "Stacked bar (time series)",
		"axes": {
				"left": {
						"mapsTo": "value",
						"stacked": true
				},
				"bottom": {
						"mapsTo": "date",
						"scaleType": "time"
				}
		},
		"height": "400px"
}
		};
	},
	template: "<ccv-stacked-bar-chart :data='data' :options='options'></ccv-stacked-bar-chart>"
};
</script>
  