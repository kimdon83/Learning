# Learning

---------

## f string
This is better than c-style and easy to use at print function.
``` python
  print( f'{df_mtrl.loc[index_mtrl][0]:15} {float(index_mtrl+1)/float(len(df_mtrl))*100:.2f}% ')
```
## Shortcuts (vscode)
1. Auto format code : ctrl + K + F
2. Hide primary side bar : ctrl + B
3. Hide Panel(Debug Concole, Terminal etc) : ctrl + J
4. Hide Activity bar : ctrl + shift + A (mine)
5. View commit history : alt + H
6. Zen Mode : ctrl + K , Z
7. Full Screen : F11
8. Move to the debug console : (Default) ctrl + shift + Y  , (mine) ctrl + M , ctrl + M 
9. (SSMS) Hide Results : ctrl + R
10.(vscode sql) excute sql : ctrl + E
11. Flip layout : Alt + Shift + 0

## VScode extensions
1. Git Graph
2. Git History
3. Todo Tree

## Git and Github
## apply()
``` python
maxlen=df_result1["mtrl"].apply(len).max()
```

---------
## IF you are using pandas and suffering from low speed.
There are some solution you can try.

1. Using iterrow
```
https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.iterrows.html
```
2. Using numpy array.
```python
df=df.to_numpy()
		# df.loc[index_mtrl*len(df_date):(index_mtrl+1) * len(df_date)-1, "BOseq"] = -1
		df[index_mtrl*len(df_date):(index_mtrl+1) * len(df_date)-1, 8] = -1
df_total=pd.DataFrame(df)
```
At first, change dataframe to numpy array. 
Change df.loc[] to df[]
Then, assign dataframe again.

## VS code - intellisence 추천이 duplicated 되었을 때 
ctrl+ ,  :-> setting 

This is related to the auto import feature (description for suggest). First suggest is auto import, second is local function (most likely). You can disable auto import by "typescript.autoImportSuggestions.enabled": false.

From <https://github.com/Microsoft/vscode/issues/38306> 
![image](https://user-images.githubusercontent.com/51689918/202035120-a60b2cad-4a0a-43ae-a1ec-9a084aa7e491.png)


df_new[df_new['l_ext'].isin([31, 22, 30, 25, 64])]
