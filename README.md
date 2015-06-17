# HW-Chipotle

import csv   
with open('chipotle.tsv','rU') as f:
    data = [row for row in csv.reader(f, delimiter='\t')]


header = data[0]
data = data[1:]

len(data)

## I thought this should work??
price = [float(row[4][1:1]) for row in data]

sum(price)/1834
