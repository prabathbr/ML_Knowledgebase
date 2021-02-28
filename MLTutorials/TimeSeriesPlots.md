# Time Series Plotting

- Ref: https://stackoverflow.com/questions/42191697/resample-daily-data-to-monthly-with-pandas-date-formatting
- Ref: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.resample.html
- Ref: https://towardsdatascience.com/using-the-pandas-resample-function-a231144194c4
- Ref: https://plot.ly/python/time-series/


### Resampling weekly:

	df_weekly = df_main.resample('W',on='date_column').sum()

### Plotting weekly:

	import plotly.graph_objects as go

	fig = go.Figure()

	for x in range(0,9,1):
	    fig.add_trace(go.Scatter(
	        x=df_weekly.index ,
	        y=df_weekly[df_weekly.columns[x]] ,
	        name=df_weekly.columns[x]
	    ))

	fig.update_layout(title_text='Weekly time-series graphs of the numeric fields',xaxis_rangeslider_visible=True)

	fig.show()