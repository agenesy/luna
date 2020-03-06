# luna

import matplotlib.pyplot as plt
import matplotlib.cbook as cbook

import numpy as np
import pandas as pd

water = pd.read_csv('water-15cm-2018-01-05T07;12;52-2018-01-19T06;14;36.205212-2018-01-19T06;14;36.205212.csv')
fname = cbook.get_sample_data('water-15cm-2018-01-05T07;12;52-2018-01-19T06;14;36.205212-2018-01-19T06;14;36.205212.csv', asfileobj=False)
with cbook.get_sample_data('water-15cm-2018-01-05T07;12;52-2018-01-19T06;14;36.205212-2018-01-19T06;14;36.205212.csv') as file:
    water= pd.read_csv(file)
    
water.plot(0, [5, 6], subplots=True)
