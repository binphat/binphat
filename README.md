#Cau 8
import pandas as pd
import numpy as np
xettuyen_df = pd.read_csv("dulieuxettuyendaihoc.csv") 
xettuyen_df["XL1"] = np.where(xettuyen_df["TBM1"]<5,Y,kY)
xettuyen_df["XL1"]

#Cau 7
import pandas as pd
import numpy as np
xettuyen_df = pd.read_csv("dulieuxettuyendaihoc.csv") 
xettuyen_df["TBM1"] = (xettuyen_df["T1"]*2 + xettuyen_df["L1"] + xettuyen_df["H1"] + xettuyen_df["S1"] + xettuyen_df["V1"]*2 + xettuyen_df["X1"] + xettuyen_df["D1"] + xettuyen_df["N1"]) / 10
xettuyen_df["TBM2"] = (xettuyen_df["T2"]*2 + xettuyen_df["L2"] + xettuyen_df["H2"] + xettuyen_df["S2"] + xettuyen_df["V2"]*2 + xettuyen_df["X2"] + xettuyen_df["D2"] + xettuyen_df["N2"]) / 10
xettuyen_df["TBM3"] = (xettuyen_df["T3"]*2 + xettuyen_df["L3"] + xettuyen_df["H3"] + xettuyen_df["S3"] + xettuyen_df["V3"]*2 + xettuyen_df["X3"] + xettuyen_df["D3"] + xettuyen_df["N3"]) / 10
xettuyen_df.to_csv("TBM.csv")
xettuyen_df

#Cau 5
import pandas as pd
import numpy as np
xettuyen_df = pd.read_csv("dulieuxettuyendaihoc.csv") 
x = xettuyen_df["T1"].median()

xettuyen_df["T1"].fillna(x, inplace = True)

xettuyen_df["T1"]



#Cau 3
import pandas as pd
import numpy as np
xettuyen_df = pd.read_csv("dulieuxettuyendaihoc.csv") 
fill_DT = xettuyen_df["DT"].fillna(int(0))
fill_DT
