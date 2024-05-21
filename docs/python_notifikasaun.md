## Uza Python hodi kalkula loron moris

Kalkula loron moris uza python.

### Vizaun Jeral

Iha topiku ida nee sei koalia konaba uza funsaun python hodi halo kalkulasaun tinan no import file no uza dataframe hodi fo sai rezultadu.

Ezemplu: Fahe subsidiu bazeia ba ema nia tinan ka ita bele hatene ohin loron ema nain hira mak selebra tinan iha instituisaun ida ka organizsaun ruma.

### Instrumentu

Instrumentu ne'ebé sei uza mak :

1. Asegura katak ita instala ona python3 iha ita nia laptop
2. Install jupyter notebook ka lab
3. Install python pandas

### Prosesu Exekuta

1. Rejistu tinan iha excel file ka source data ruma ne'ebe rejistu ho data moris ezemplu hanesan `No`, `Municipio`, `Posto`, `Suco`, `Aldeia`, `Naran`,` Ke-BI`, `Data-Moris` no save ho tipu format csv iha diretory nebe ita atu halo kalkulasaun.

2. Loke Jupyter lab iha terminal `jupyter lab`

   ```
   (saturday_2024) ➜  saturday_2024 jupyter lab
   [I 2024-02-25 11:28:16.006 ServerApp] jupyterlab | extension was successfully linked.
   [I 2024-02-25 11:28:16.736 ServerApp] nbclassic | extension was successfully linked.
   ```

3. Kria file jupyter ida ho naran `kalkula_tinan` hamutuk ho file excel nebe ita rai hanesan file csv.

4. **Flowchart 1 konaba prosesu kalkula tinan.**

   ```mermaid
   flowchart LR
       A([Inisia]) --> B(Kria funsaun)
       B --> C{Deklara kondisaun}
       C --> D[(Check data iha database)]
       D -->|Sin| E[Aprova]
       D -->|Lae| F[La aprova]
   ```

   

   4.1. Import python library
```
  import pandas as pd
  from datetime import datetime
  from datetime import date
```
​       4.2. Kria data variabel ida ho tipu dictionary no hatama ba data frame
```
 d = {
    "No": [1, 2, 3], 
    "Naran": ["Mario", "Antonio", "Joanico"], 
    "data_moris": ['17.02.1960', '27.02.1961', '07.01.1991']
}
df = pd.DataFrame(data=d) 
```

​       4.3. Kria funsaun konaba kalkula tinan.
```
  def kalkula_tinan(data_moris):
      born = datetime.strptime(data_moris, "%d.%m.%Y").date()
      today = date.today()
      return today.year - born.year - ((today.month, today.day) < (born.month, born.day))
```
   4.4. Deklara kondisaun.
```
  def notifikasaun(tinan):
      if tinan == 60:
        return "Parabens Ohin Ita hetan ona subsidu"
      elif tinan >= 60:
        return "Ita hetan ona subsidu"
      elif tinan <= 60:
        return "Favor hein ita nia subsidu"
```

​	4.5. Exekuta python no fo sai rezultadu
```
  df['age'] = df['data_moris'].apply(kalkula_tinan)
  df['mensajen'] = df['age'].apply(notifikasaun)
  df
```
Rezultadu:   

|No	|Naran	|data_moris	|age	|mensajen            |
|-----|--------|-----------|-----|--------------------|
|1	   |Mario	|17.02.1960	|64	|Ita hetan ona subsidu|
|2	   |Antonio	|27.02.1961	|63	|Ita hetan ona subsidu|
|3	   |Joanico	|07.01.1991	|33	|Favor hein ita nia subsidu|

5. **Flowchart 2 konaba import csv file no uza panda data frame hodi kalkula tinan.**

   
  
   ```mermaid
   flowchart LR
   		P[[Oinsa hatama scv file uza pandas data frame?]]
       P --> A
       A([Hatama data]) --> B(Kria funsaun ida)
       B --> C{Deklara kondisaun} 
       C -->|Sin| D[Aprova]
       C -->|Lae| E[La aprova]
   ```
   
   
   
   5.1 Import python library

```
   from datetime import datetime
   from datetime import date
   import pandas as pd
   df = pd.read_csv('naran.csv', sep=';')
```
 	5.2 Kria funsaun konaba kalkula tinan.
```     
   # Kria funsaun Kalkula tinan
   def kalkula_tinan(data_moris):
       # kria tipu format tinan nian
       born = pd.to_datetime(data_moris, format="%Y-%m-%d")
       today = date.today()
       # kalkula tinan moris ho data ohin nian
       return today.year - born.year - ((today.month, today.day) > (born.month, born.day))
```
​	 5.3 Kria funsaun ida konaba notifikasaun tinan moris nian.
```
   # Kria funsaun haruka konaba tinan
   def notifikasaun(tinan):
       if tinan == 60:
           return "Parabens Ohin Ita hetan ona subsidu"
       elif tinan >= 60:
           return "Ita hetan ona subsidu"
       elif tinan <= 60:
           return "Favor hein ita nia subsidu"
```
​	5.4 Exekuta rezultadu ho python 
```
   # kria koluna foun ho naran tinan no aplika tinan
   df['tinan'] = df['Loron_Moris'].apply(kalkula_tinan)
   df['mensajen'] = df['tinan'].apply(notifikasaun)
     
   #print valor espesifiku.
   df = df.loc[df['tinan'] == 60]
```
​	5.5 Kria file csv foun husi rezultadu:
```
   #kria csv file
   df = df.to_csv("tinan.csv", encoding='utf-8', index=False)
   df 
```
### Rezultadu

​       ![resulatufinal](https://i.postimg.cc/DwkqqJ4v/Screen-Shot-2021-03-18-at-4-23-21-PM.png)

​       