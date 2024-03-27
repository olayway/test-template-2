---
datapackage:
  title: Dataset Template
  description: A template for a dataset to publish on DataHub. Uses the Data Package metadata.
  licenses:
  - path: http://opendatacommons.org/licenses/pddl/
    title: Open Data Commons Public Domain Dedication and License v1.0
  resources:
  - path: data.csv
    title: C02 PPM per decade
    name: c02-per-decade
    format: csv
    schema:
      fields:
      - name: year
        type: date
      - name: co2
        type: number
---

Here's some text.

You can add as much text as you like.

The data files will be automatically displayed here.

We can add a chart:

<LineChart
  data="./data.csv"
  title="C02 per decade"
  xAxis="year"
  yAxis="co2"
/>


<PlotlyLineChart
  data={[
    {
      temperature: -0.41765878,
      year: '1850'
    },
    {
      temperature: -0.2333498,
      year: '1851'
    },
    {
      temperature: -0.22939907,
      year: '1852'
    },
    {
      temperature: -0.27035445,
      year: '1853'
    },
    {
      temperature: -0.29163003,
      year: '1854'
    }
  ]}
  xAxis="year"
  yAxis="temperature"
/>

LINE CHART URL

<PlotlyLineChart
  url="./data.csv"
  xAxis="year"
  yAxis="co2"
/>


<PlotlyBarChart
  data={[
    {
      temperature: -0.41765878,
      year: '1850'
    },
    {
      temperature: -0.2333498,
      year: '1851'
    },
    {
      temperature: -0.22939907,
      year: '1852'
    },
    {
      temperature: -0.27035445,
      year: '1853'
    },
    {
      temperature: -0.29163003,
      year: '1854'
    }
  ]}
  xAxis="year"
  yAxis="temperature"
/>

<PlotlyBarChart
  url="./data.csv"
  xAxis="year"
  yAxis="co2"
/>

<Plotly
  data={[
    {
      marker: {
        color: 'red'
      },
      mode: 'lines+markers',
      type: 'scatter',
      x: [
        1,
        2,
        3
      ],
      y: [
        2,
        6,
        3
      ]
    }
  ]}
  layout={{
    title: {
      text: 'Chart built with Plotly'
    },
    xaxis: {
      autorange: true,
      range: [
        0.8714733542319749,
        3.128526645768025
      ],
      title: {
        text: 'x Axis'
      },
      type: 'linear'
    },
    yaxis: {
      autorange: true,
      range: [
        1.7070063694267517,
        6.292993630573249
      ],
      title: {
        text: 'y Axis'
      },
      type: 'linear'
    }
  }}
/>

<Plotly
  data="./data.csv"
  layout={{
    title: {
      text: 'Chart built with Plotly'
    },
    xaxis: {
      autorange: true,
      range: [
        0.8714733542319749,
        3.128526645768025
      ],
      title: {
        text: 'x Axis'
      },
      type: 'linear'
    },
    yaxis: {
      autorange: true,
      range: [
        1.7070063694267517,
        6.292993630573249
      ],
      title: {
        text: 'y Axis'
      },
      type: 'linear'
    }
  }}
/>
