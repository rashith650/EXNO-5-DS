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
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label="line 1")

x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="line 2")

plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph')

plt.legend()
```
![image](https://github.com/user-attachments/assets/4f3a5381-e210-441b-aa7d-0d62119bb36f)

```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('some cool!')
```
![image](https://github.com/user-attachments/assets/e599be42-542e-4cbe-a3a0-3a6767172b76)

```
yield_apples = [0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
![image](https://github.com/user-attachments/assets/e45e8828-8819-44a0-b50a-79b9babdb0e3)

```
years=[2010,2011,2012,2013,2014,2015]
yield_apples = [0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```
![image](https://github.com/user-attachments/assets/bdad12eb-ed9d-409a-a1e8-5f6b0def0976)

```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.962,0.941,0.930,0.923,0.918,0.900,0.907,0.904,0.901,0.898,0.9,0.896]
plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel("year")
plt.ylabel("Yield(toes per hectare)");
```
![image](https://github.com/user-attachments/assets/3892ff26-9abd-4c76-8bb2-efb112ca99e4)

```
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g*--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
```
![image](https://github.com/user-attachments/assets/ddaf0934-54d9-45a5-99b3-5e4767743966)

```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color="blue")
plt.fill_between(x,y2,color="green")
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
```
![image](https://github.com/user-attachments/assets/b0325636-111b-4c05-ab22-c7b7edad6854)

```
import matplotlib.pyplot as plt
values=[5,6,3,7,2]
names=["A","B","C","D","E"]

plt.barh(names,values,color="yellowgreen")
plt.show()
```
![image](https://github.com/user-attachments/assets/622f189e-147f-4c81-83a4-d51b20cf63ae)
```
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()
```
![image](https://github.com/user-attachments/assets/058a4096-2c49-4648-8165-7fed44656ecc)
```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```
![image](https://github.com/user-attachments/assets/6fb7cfcf-3b6a-4367-bfbb-9d983a239879)
```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No.of people')
plt.title('My histogram')
plt.show()
```
![image](https://github.com/user-attachments/assets/d340b31d-561d-4407-81e4-3607be4d48aa)
```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![image](https://github.com/user-attachments/assets/ae27b4a6-d56c-4e49-b279-14db01c5f691)
```
import matplotlib.pyplot as plt
x=[2,1,6,2,4,8,9,4,2,4,10,6,4,5,7,7,3,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color='blue',alpha=0.5)
plt.show()
```
![image](https://github.com/user-attachments/assets/492ac511-e41f-40e1-b94d-5b35af8a9fc3)
```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box plot')
```
![image](https://github.com/user-attachments/assets/ad1b2cc4-9c29-46e8-a441-20e912a1c5a9)
```
import matplotlib.pyplot as plt
activities = ['eat', 'sleep', 'work', 'play']
slices =[3, 7, 8, 6]
colors = ['r', 'y', 'g', 'b'] 
plt.pie (slices, labels=activities, colors=colors, startangle=90, shadow= True, explode =(0, 0, 0.1, 0), radius= 1.2, autopct = '%1.1f%%')
plt.legend ()
plt.show()
```
![image](https://github.com/user-attachments/assets/bd4b7ee8-d8cb-4c3d-af62-15db65c58396)
```

labels ='Python', 'C++', 'Ruby', 'Java'
sizes =[215, 138, 245, 210]
colors= ['gold', 'yellowgreen', 'lightcoral', 'lightskyblue'] 
explode = (0, 0.4, 0, 0.5)

plt.pie(sizes, explode=explode, labels =labels, colors=colors, autopct='%1.1f%%', shadow=True)
plt.axis('equal')
plt.show()
```
![image](https://github.com/user-attachments/assets/3b8da03f-4c33-4c6b-80ad-6434fd389e1c)


# Result:
Thus the program to Perform Data Visualization using matplot python library for the given datas is been implemented.
