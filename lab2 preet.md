# Lab 2


### function 1:

Analyze the following function with respect to number

```python
def function1(number):
	total=0;	#1

	for i in range(0,number):	#n
		x = (i+1)		#2n
		total+=(x*x)	#2n

	return total #1
```

$$T(n) = 1 + n + 2n + 2n + 1 = 5n + 2$$

$$T(n)\hspace{0.2cm}\text{is}\hspace{0.2cm} O(n)$$
### function 2:

Analyze the following function with respect to number

```python
def function2(number):
	return  ((number)*(number+1)*(2*number + 1))/6 #7

```
$$T(n) = 7$$

$$T(n)\hspace{0.2cm}\text{is}\hspace{0.2cm} O(1)$$

### function 3:

Analyze the following with respect to the length of the list.  Note that the function call len() which returns the length of the list is constant (O(1)) with respect to the length of the list.
```python

def function3(list):
	for i in range (0,len(list)-1):      #n-1
		for j in range(0,len(list)-1-i): #0.5n^2 + 3.5n - 3 (proof given below)
			if(list[j]>list[j+1]):	#3.5n^2 +3.5n (proof given below)
				tmp=list[j]			
				list[j]=list[j+1]	
				list[j+1]=tmp

```

Proof of number of operations peformed in if
![alt text](./images/images.png)
Proof of number of iterations of inner for loop
![alt text](./images/forImage.png)
![alt text](./images/finalFunction3.png)

### function 4:

Analyze the following function with respect to number

```python
def function4(number):
	total=1 #1
	for i in range(1 to number): #n-1
		total=total*(i+1) #3(n-1)
	return total #1
```
$$T(n) = 1 + n-1 + 3(n-1) + 1$$
$$= 4n + 4$$
$$T(n)\hspace{0.2cm}\text{is}\hspace{0.2cm} O(n)$$



## In class portion


### Group members
List the members of your group member below:

	* Name 
	* Preet Patel
	* Angelo Gatto
	* Vrunda Patel

### Timing Data

grab a screenshot of your excel graphs and put it here

#### partb_one
![alt text](./images/1.png)
#### partb_two

#### partb_three
![alt text](./images/3.jpeg)
### Summary 
|function| runtime based on analysis | Most similar curve | 
|---|---|---|
|partb_one()| $$\text{Quadratic}\hspace{0.2cm}O\left(  n^{2}\right)$$ | Quadratic |
|partb_two()| $$\text{Logarithmic}\hspace{0.2cm}O\left( n\log n\right)$$    |   |
|partb_three()| $$\text{Linear}\hspace{0.2cm}O\left(  n\right)$$  | Linear  |


### Discussion:

Look at the code from lab 1 and discuss the differences between fastest/slowest versions. Was it a difference in syntax? A difference in approach?  Write down your observations.


## Reflection:

1. for each function what growth rate best match your results?
For the first function i.e.

	| Function Name | Growth Rates |
	|---|---|
	| partb_one() | $$O\left(  n^{2}\right)$$ |
	| partb_two() | $$O\left( n\log n \right)$$ |
	| partb_three() | $$O\left( n \right)$$|


2. Does your analysis match your analysis?  If not, where do you suppose the error occurred?


	Our group's analysis based on graph and based on the 5 	step method does match and there were not any errors. However, we saw that graphs were not completely following the theoretical path. For instance the first function had a time complexity of n^2 so the relation between amount of data and time should be y=n^2 however this was not the case for all the values of amount of data and time there were cases where the increase in the amount of data was not equals to the square of time but all these deflections/errors are understandable as for larger amounts of data these deflections would be insignificant. 
3. What sort of conclusions can you draw based on your observations?	
	
	
	Based on these observations, we can conclude that the curve plotted using real-time analysis will not exactly match the theoretical curve. However, it will approximate the theoretical curve closely.  and hence we can say that whilst calculating time complexity precision is not important for larger amounts of data 




