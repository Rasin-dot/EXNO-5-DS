# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```

# LINE PLOT
```
marks=[13,45,63,78]
 student=['ABC','QOR','EFB','TOB']
 plt.plot(marks,student)
 plt.xlabel('Marks')
 plt.ylabel('Student name')
 plt.show()
 student=['A','B','C','D']
 attendence=[90,85,73,88]
 plt.plot(attendence,student)
 plt.xlabel('Attendence')
 plt.ylabel('Student name')
 plt.show()
```

# OUTPUT


<img width="778" height="815" alt="504607055-6018e45e-a3c1-4f54-903a-9b65757e181d" src="https://github.com/user-attachments/assets/873ccf12-9c83-4afc-befd-4a09d061bc98" />


# SCATTER  PLOT

```
 x=[10,20,30,40,50]
 y=[100,200,300,400,500]
 plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
 plt.show()
 x=np.arange(0,15)
 y=np.arange(0,15)
 x
 y
 plt.scatter(x,y,c='r')
 plt.xlabel('X axis')
 plt.ylabel('y axis')
 plt.title('Scatter plot')
 plt.show()

```

# OUTPUT 

<img width="665" height="836" alt="504608206-939cf818-3363-48cc-a3a8-e072e4eae829" src="https://github.com/user-attachments/assets/fa537226-cbbd-48fc-9feb-59ef32ef7cc5" />


# PIE CHART

```
act=['eat','sleep','work','play']
 slices=[3,7,8,6]
 color=['r','y','g','b']
 plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
 plt.legend()
 plt.show()
 feedback=['Good','excellent','Perfect','Ok']
 slices=[4,10,3,8]
 color=['y','r','b','g']
 plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
 plt.legend()
 plt.show()
```


# OUTPUT 

<img width="778" height="778" alt="504608827-7712f1de-44ac-42f9-9bab-a3908c7c2786" src="https://github.com/user-attachments/assets/ae5432b0-1fef-4772-b9fd-e72da91f4a52" />


# AREA CHART

```
 x = [1, 2, 3, 4, 5]
 y1 = [10, 12, 14, 16, 18]
 y2 = [5, 7, 9, 11, 13]
 y3 = [2, 4, 6, 8, 10]
 plt.fill_between(x, y1, color='blue')
 plt.fill_between(x, y2, color='green')
 plt.plot(x, y1, color='red')
 plt.plot(x, y2, color='black')
 plt.legend(['y1','y2'])
 plt.show()

```

# OUTPUT 

<img width="694" height="463" alt="504609850-94355db8-128a-4d62-a047-02aa738c2cd5" src="https://github.com/user-attachments/assets/4527b0e7-3bad-447b-8bac-1b7bff3f439f" />


# BAR CHART 

```
height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green'] 
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()
```

# OUTPUT 


<img width="611" height="484" alt="504610978-ee1c1cb0-c425-498e-83bb-78ce5a5d6817" src="https://github.com/user-attachments/assets/05df46e8-e5c7-4857-ae8f-df5aef51bde1" />


# HISTOGRAM 

```
 x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
 plt.hist(x, bins = 10, color='blue')
 plt.show()
```

# OUTPUT

<img width="548" height="367" alt="504611431-67f2d11f-92db-4e44-b68c-a9834d985936" src="https://github.com/user-attachments/assets/30d5c2ad-0b51-4dc3-83a3-d29460113064" />


```
 x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
 plt.hist(x, bins = 10, color='blue', alpha=0.3)
 plt.show()
```

# OUTPUT



<img width="628" height="366" alt="504612148-ff93a1e2-21c2-4e79-833c-8dfcc59dd57f" src="https://github.com/user-attachments/assets/3233e0bf-2b10-414a-a83d-bd3c771e1b28" />

# BOX PLOT
```
np.random.seed(0)
 data=np.random.normal(loc=0, scale=1, size=100)
 data
```

# OUTPUT

<img width="653" height="316" alt="504612415-976d9bb0-ebcb-498c-b735-7e511311adaa" src="https://github.com/user-attachments/assets/83092f09-88cc-47d6-8d26-37883010028d" />


```
 fig, ax= plt.subplots()
 ax.boxplot(data)
 ax.set_xlabel('Data')
 ax.set_ylabel('Values')
 ax.set_title('Box Plot')

```

# OUTPUT 


<img width="739" height="456" alt="504612891-674b1300-288a-44fe-944f-d1a71dce0f8a" src="https://github.com/user-attachments/assets/b6223b5c-add6-467f-93ac-c68917405b07" />








# Result:
Thus, all the data visualization techniques of matplotlib has been implemented.
