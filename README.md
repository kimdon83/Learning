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

--
