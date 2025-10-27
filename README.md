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
## Name: Chiiradeep R
## Reg no: 212224240028
```py
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```
## Line Plot:
~~~py
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
~~~
<img width="944" height="549" alt="image" src="https://github.com/user-attachments/assets/297eadc8-7eec-4d17-b09b-247feec91aa0" />

<img width="819" height="528" alt="image" src="https://github.com/user-attachments/assets/5646cbce-cbd1-401c-8123-a833a2dcdbc0" />

## Scatter Plot:
~~~py
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
~~~

<img width="875" height="553" alt="image" src="https://github.com/user-attachments/assets/1b2fb3c4-efa2-49fa-9e17-8e4a619be530" />

<img width="743" height="533" alt="image" src="https://github.com/user-attachments/assets/51fe0deb-9539-469d-b14e-4b7d2c1b4e37" />

## Pie Chart:
~~~py
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
~~~

<img width="769" height="527" alt="image" src="https://github.com/user-attachments/assets/f8af0005-78b1-426d-8b37-7ae59bbe55be" />

<img width="732" height="540" alt="image" src="https://github.com/user-attachments/assets/cf74aec6-2764-43c9-986b-46a8e51d5018" />

## Area Chart:
~~~py
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
~~~

<img width="1018" height="551" alt="image" src="https://github.com/user-attachments/assets/8eb8b600-5a76-473b-be36-1673088cec7f" />

## Bar Chart:

~~~py
height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green']
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()
~~~

<img width="984" height="608" alt="image" src="https://github.com/user-attachments/assets/7d881f08-7fce-4c60-ab9e-24d5bd48a177" />

## Histogram:
~~~py
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
~~~

<img width="995" height="542" alt="image" src="https://github.com/user-attachments/assets/6397d1ba-9b78-47a2-8fab-8d58ad894638" />

## Box Plot:

~~~py
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
~~~

<img width="1016" height="463" alt="image" src="https://github.com/user-attachments/assets/e53cc29b-0194-45c1-91ae-b40a33b3322a" />

~~~py
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
~~~

<img width="886" height="614" alt="image" src="https://github.com/user-attachments/assets/bbccca47-a228-40de-9635-93628321b8f5" />

# Result:
Thus, all the data visualization techniques of matplotlib has been implemented
