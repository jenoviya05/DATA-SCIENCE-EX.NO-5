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
 ~~~
import matplotlib.pyplot as plt

%matplotlib inline
import numpy as np
x=np.arange(0,10)
y=np.arange(11,21)
a=np.arange(40,50)
b=np.arange(50,60)
plt.scatter(x,y,c='g')
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
~~~

<img width="563" height="455" alt="image" src="https://github.com/user-attachments/assets/03d38087-c0cb-4ce5-853d-e67c808f698e" />

~~~
y=x*x
plt.plot(x,y,'r*',linestyle='dashed',linewidth=2, markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
plt.show()
~~~

<img width="562" height="455" alt="image" src="https://github.com/user-attachments/assets/ccc5c17f-9e58-464c-aa79-c0b2d852fcb9" />

~~~
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g*--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
plt.show()
~~~

<img width="543" height="413" alt="image" src="https://github.com/user-attachments/assets/ea31f888-fce0-4c71-8d26-4e6496bc0062" />

~~~
x = np.arange(1,11) 
y = 3 * x + 5 
plt.title("Matplotlib demo") 
plt.xlabel("x axis caption") 
plt.ylabel("y axis caption") 
plt.plot(x,y) 
plt.show()
~~~

<img width="562" height="455" alt="image" src="https://github.com/user-attachments/assets/0a9ab25d-9600-430d-bc51-02160092c7eb" />

~~~
np.pi
~~~

<img width="235" height="66" alt="Screenshot 2026-03-09 225535" src="https://github.com/user-attachments/assets/8cbbbdff-b7ce-4351-87ff-a6a974f69f87" />

~~~
# Compute the x and y coordinates for points on a sine curve 
x = np.arange(0, 4 * np.pi, 0.1) 
y = np.sin(x) 
plt.title("sine wave form") 

# Plot the points using matplotlib 
plt.plot(x, y) 
plt.show()
~~~


<img width="568" height="435" alt="image" src="https://github.com/user-attachments/assets/0d975008-33d4-41bd-8b50-e812ecb3eb64" />

~~~
#Subplot()
# Compute the x and y coordinates for points on sine and cosine curves 
x = np.arange(0, 5 * np.pi, 0.1) 
y_sin = np.sin(x) 
y_cos = np.cos(x)  
   
# Set up a subplot grid that has height 2 and width 1, 
# and set the first such subplot as active. 
plt.subplot(2, 1, 1)
   
# Make the first plot 
plt.plot(x, y_sin,'r--') 
plt.title('Sine')  
   
# Set the second subplot as active, and make the second plot. 
plt.subplot(2, 1, 2) 
plt.plot(x, y_cos,'g--') 
plt.title('Cosine')  
   
# Show the figure. 
plt.show()
~~~

<img width="559" height="435" alt="image" src="https://github.com/user-attachments/assets/1133e979-936d-407c-9e90-1fb41e8494e2" />

~~~
## Bar plot

x = [2,8,10] 
y = [11,16,9]  

x2 = [3,9,11] 
y2 = [6,15,7] 
plt.bar(x, y) 
plt.bar(x2, y2, color = 'g') 
plt.title('Bar graph') 
plt.ylabel('Y axis') 
plt.xlabel('X axis')  

plt.show()
~~~

<img width="563" height="455" alt="image" src="https://github.com/user-attachments/assets/d236e717-9939-4361-9315-e70e35a9a073" />

~~~
a = np.array([22,87,5,43,56,73,55,54,11,20,51,5,79,31,27]) 
plt.hist(a) 
plt.title("histogram") 
plt.show()
~~~

<img width="547" height="435" alt="image" src="https://github.com/user-attachments/assets/694e05ae-354c-4b7e-ad44-e79c09010aa7" />

~~~
data = [np.random.normal(0, std, 100) for std in range(1, 4)]

# rectangular box plot
plt.boxplot(data,vert=True,patch_artist=False);  
plt.show()
~~~

<img width="546" height="413" alt="image" src="https://github.com/user-attachments/assets/4065d072-5140-4306-ad58-d7e5588ff88c" />

~~~
data = [np.random.normal(0, std, 100) for std in range(1, 4)]

# rectangular box plot
plt.boxplot(data,vert=True,patch_artist=True);
plt.show() 
~~~

<img width="546" height="413" alt="image" src="https://github.com/user-attachments/assets/7f96da68-20ba-4481-8af3-575f57a03473" />

~~~
data
~~~

<img width="801" height="805" alt="Screenshot 2026-03-09 225936" src="https://github.com/user-attachments/assets/0a4867f5-d3fe-41aa-a5cd-17ebb1fe694b" />

~~~
# Data to plot
labels = 'Python', 'C++', 'Ruby', 'Java'
sizes = [215, 130, 245, 210]
colors = ['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode = (0.4, 0, 0, 0)  # explode 1st slice

# Plot
plt.pie(sizes, explode=explode, labels=labels, colors=colors,
autopct='%1.1f%%', shadow=False)

plt.axis('equal')
plt.show()
~~~

<img width="515" height="389" alt="image" src="https://github.com/user-attachments/assets/aed1fdc2-07d6-403f-add8-a2d1d51abdb1" />


# Result:

     Thus Data Visualisation using matplotlib library has been done and verified.
