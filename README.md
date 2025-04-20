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
# Coding and Output:
import matplotlib.pyplot as plt

x1=[1,2,3]

y1=[2,4,1]

plt.plot(x1,y1, label="line 1", linewidth=6)

x2=[1,2,3]

y2=[4,1,3]

plt.plot(x2,y2, label="line 2", linewidth=6)

plt.xlabel('X-AXIS')

plt.ylabel('Y-AXIS')

plt.title("Two lines on same graph")

plt.legend()

![image](https://github.com/user-attachments/assets/1d55b918-e645-4c6e-a3fa-5e03840b3bfa)

import matplotlib.pyplot as plt

x=[1,2,3,4,5,6]

y=[2,4,1,5,2,6]

plt.plot(x,y,color='blue', linestyle='dashed', linewidth=4, marker='o', markerfacecolor='red', markersize=14)

plt.ylim(1,8)

plt.xlim(1,8)

plt.xlabel('X-AXIS')

plt.ylabel('Y-AXIS')

plt.title('Some Cool Customizations')

![image](https://github.com/user-attachments/assets/14169066-e6b7-40cf-bc11-1dc8f0b53daa)

years =range(2000, 2012)

apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]

oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896,]

plt.plot(years, apples, color='red', linewidth=5)

plt.plot(years, oranges, color='orange', linewidth=5)

plt.xlabel('YEAR')

plt.ylabel('Yields (tons per hectare)')

plt.title('Crop Yields in Kanto')

plt.legend(['Apples', 'Oranges'])

![image](https://github.com/user-attachments/assets/788803ac-50cc-449c-bf69-344ac633269c)

import matplotlib.pyplot as plt

x_values=[0,1,2,3,4,5]

y_values=[0,1,4,9,16,25]

plt.scatter(x_values,y_values,s=100,c='red')

plt.xlabel('X-AXIS')

plt.ylabel('Y-AXIS')

plt.title('Scatter Plot')

![image](https://github.com/user-attachments/assets/68cacb6b-08c7-4eaa-b655-a665723b3d51)


import matplotlib.pyplot as plt

x_values=[1,2,3,4,5,6,7,8,9,10]

y_values=[2,4,5,7,6,8,9,11,12,12]

plt.scatter(x_values,y_values, label='stars', marker='*',s=300,c='blue')

plt.xlabel('X-AXIS')

plt.ylabel('Y-AXIS')

plt.title('Scatter Plot Star')

plt.legend()

plt.savefig("StarScatter.png")

![image](https://github.com/user-attachments/assets/f6a96fe5-a5a0-4178-9299-4e0ce9b1c2de)

import matplotlib.pyplot as plt

x= [1,2,3,4,5,6,7,8,9]

y=[1,4,9,16,25,36,49,64,81]

plt.xlabel('X-AXIS')

plt.ylabel('Y-AXIS')

plt.title('Scatter Plot Star')

plt.subplot(2,2,1)

plt.plot(x,y, 'ro--')

plt.subplot(2,2,2)

plt.plot(y,x, 'g*--')

plt.subplot(2,2,3)

plt.plot(x,x, 'bo')

plt.subplot(2,2,4)

plt.plot(y,y, 'go')

![image](https://github.com/user-attachments/assets/66d201a9-6240-469c-a8d4-f7db59e06ed1)

import numpy as np

np.pi

![image](https://github.com/user-attachments/assets/fc8b90ff-c97d-4b02-8024-04e5e06f08ed)

X=np.arange(0,4*np.pi,0.1)

Y=np.sin(X)

plt.title("Sin Wave Form")

plt.plot(X,Y, linewidth=5,c='green', linestyle='dotted')

![image](https://github.com/user-attachments/assets/7d9f662d-9acc-4d48-87d8-04c5bfecc1ea)

import matplotlib.pyplot as plt

import numpy as np

x= [1,2,3,4,5]

y1=[10,12,14,16,18]

y2=[5,7,9,11,13]

y3=[2,4,6,8,10]

plt.fill_between (x,y1, color='red')

plt.fill_between (x,y2, color='blue')

plt.plot(x,y1, color='black')

plt.plot(x,y2, color='white')

plt.legend(['y1','y2'])

plt.show()

![image](https://github.com/user-attachments/assets/d761e61f-475c-4e2a-ba85-e6528bebbeae)

import matplotlib.pyplot as plt

height=[10,24,36,40,5]

names=['One', 'Two', 'Three', 'Four', 'Five']

c1=['g','b']

plt.bar(names, height, width=0.8,color=c1)

plt.xlabel('X-AXIS')

plt.ylabel('Y-AXIS')

plt.title('Bar Graph')

![image](https://github.com/user-attachments/assets/0e581f69-82fe-4326-b1fe-315deaa82fb5)

x = [2, 8, 10]

y = [11, 16, 9]

x2 = [3, 9, 11]

y2 = [6, 15, 7]

plt.bar(x,y,color='r')

plt.bar(x2,y2,color='y')

plt.xlabel('X-AXIS')

plt.ylabel('Y-AXIS')

plt.title('Bar Graph')

![image](https://github.com/user-attachments/assets/a93b939c-931a-4087-be17-ff2656d7bdc2)

import matplotlib.pyplot as plt

ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90, 77, 32, 21, 20, 40]

range=(0,100)

bins=10

plt.hist (ages, bins, range, color='orange', histtype='bar', rwidth=0.8)

plt.xlabel('age')

plt.ylabel('no.of people')

plt.title('Histogram')

![image](https://github.com/user-attachments/assets/2d6c377a-1ee8-4d37-abc3-35beb5c0d593)

import matplotlib.pyplot as plt

x= [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]

plt.hist(x,bins=10,color='grey', alpha=0.5)

plt.show()

![Screenshot 2025-04-19 194119](https://github.com/user-attachments/assets/c682060c-3d4c-4d50-8838-c01dc32c0ddf)

import matplotlib.pyplot as plt

import numpy as np

np.random.seed(0)

data=np.random.normal(loc=0,scale=1,size=100)

data

![image](https://github.com/user-attachments/assets/0100c9f7-ab70-4b01-bbd6-84c2f8ed8dd6)


fig,ax=plt.subplots()

ax.boxplot(data)

ax.set_xlabel('Data')

ax.set_ylabel('Value')

ax.set_title('Box Plot')

![image](https://github.com/user-attachments/assets/b2730ecc-c76d-4112-8a8a-018abf88503f)

import matplotlib.pyplot as plt

activities=['Eat', 'Sleep', 'Work', 'Play']

slices=[3,7,8,6]

colors=['yellow', 'blue', 'orange', 'red']

plt.pie(slices,labels=activities, colors=colors, startangle=90,shadow=True, explode=(0,0.1,0,0), autopct='%1.1f%%')

plt.title('Pie Chart')

plt.show()

![image](https://github.com/user-attachments/assets/4062645f-7a12-4e81-b077-c6e454d1bb79)

labels=['Python', 'C++', 'Ruby', 'Java']

sizes=[215,130, 245, 210]

colors=['orange', 'yellow', 'red', 'blue']

explode=(0.1,0,0.1,0)

plt.pie(sizes,explode=explode, labels=labels, colors=colors, autopct='%1.1f%%', shadow=True, startangle=90)

plt.axis('Equal')

plt.show()

![image](https://github.com/user-attachments/assets/78d84d96-5f6e-429a-b506-3964c164ee39)

# Result:
 Thus the program to Perform Data Visualization using matplot python library for the given datas is
 been implemented.

