# data-visualization
WHO-COVID-19-global-table-data
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt

data = pd.read_csv(r"C:\Users\dell\Downloads\WHO-COVID-19-global-table-data.csv")

data

data.head()

data.columns

data.tail

data.describe

# data visualization by scatter plots

data.columns

sns.relplot(x="Cases - newly reported in last 7 days",y="Deaths - newly reported in last 7 days",data=data)

sns.relplot(x="C",y="Deaths - cumulative total",hue ="Cases - newly reported in last 24 hours",data=data)

# line plot


sns.relplot(x="Cases - newly reported in last 7 days",y="Deaths - newly reported in last 7 days",kind="line",data=data)

data.columns


sns.relplot(x="Name",y="WHO Region",kind="line",data=data)

sns.relplot(x="Name",y="WHO Region",hue ="Cases - cumulative total",kind="line",data=data)



