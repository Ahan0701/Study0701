# Computer Science

### Linear Regression
Linear Regression is a linear equation used for predicting a value of something when there are multiple data sets with a different rate of change. Regression analysis stems from the idea that given data have a certain tendency. The main purpose of regression analysis is to explain the tendency among variables. When expressed mathematically, the regression model is divided into a part that shows a trend and a part that shows an uncontrollable error. The equation has the form Y= a + bX, where Y is the dependent variable, X is the independent variable, b is the slope of the line, and a is the y-intercept.
[logo]: https://miro.medium.com/max/1400/1*Cw5ZSYDkIFpmhBwr-hN84A.png "Linear Regression"

### Derivative
A derivative represents the slope of the tangent line at a specific point on the curve. In the case of a straight line, the slope does not change even if x changes because it continues to extend in the same direction. But, because the slope changes depending on what the value of x is on a curved line, we differentiate to find the value of the slope that changes according to the value of x. The equation obtained by differentiating the cubic function is the equation for the slope. You just need to find two x-values where the value at that time is 0 and draw a graph around that value. This point is specifically called the inflection point, and the y-value at this point is called the extreme point. Extreme points are places where a function takes on an extreme value, a value that is especially small or especially large compared to other nearby values of the function. When the slope is a negative number, the graph is convex up. In this case, the top tip of this convex is the extreme point. When the slope is a positive number, it is convex down. In this case, the bottom tip of this convex is the extreme point. 
[logo]: https://www.mathfactory.net/wp-content/uploads/%EC%88%98%ED%95%99-%EA%B3%B5%EC%8B%9D-%ED%8F%89%EA%B7%A0%EB%B3%80%ED%99%94%EC%9C%A8-%EB%AF%B8%EB%B6%84%EA%B3%84%EC%88%98-02.png "Derivative"

### a b
y^i=axi+b
∑ei^2=∑(yi-axi-b)^2

partial derivative for b: 
∂∑ei^2/∂b=2∑(-1)(yi-axa-b)

When this equation is 0: 
0=∑yi-a∑xi-nb

nb=∑yi-a∑xi

b=∑yi-a∑xi/n

When average if yi=￣y:

b=￣y-a(￣x)
	
Partial derivative for ∑R:

y∑∂i^2/∂i= (-1)2∑(yi-axi-b)(xi)
	
0=-2{∑yi-xi-a∑(xi^2)-b∑xi}

a∑(xi^2)=∑(yi)xi-b∑xi	

a{∑(xi^2)-￣∑xi}=∑yi(xi)-￣yxi

a=∑ti(xi)-￣y∑xi/∑(xi^2)-￣x∑xi


### MSE and RMSE
MSE=1/n∑(y-y^)^2

RMSE=√mse=√∑(y^-y)^2/n

MSE represents the difference between the original and predicted values extracted by squaring the mean difference over a data set. MSE is the measure of how close the fitted line is to the actual data points. The closer the fit is to the data set if the smaller the mean squared error. MSE has units squared on the vertical axis. RMSE is the error rate by the square root of MSE. RMSE is the easiest statistic to interpret because it has the same units as the values shown on the vertical or y-axis. It is a better measure of goodness of fit than correlation coefficient because RMSE can be interpreted directly as a unit of measure. 

### R^2
R^2=1-RSS/TSS

R^2 is the coefficient of determination. Let's look at the coefficient of determination (R^2). This is what is commonly called R squared.  R^2 is a measure of how well the estimated linear model fits the given data. The proportion of the variance of the response variable (y) can be explained by the fitted model. The coefficient of determination is an indicator of how much the independent variable explains the dependent variable in a regression model. Also called explanatory power. 

A higher coefficient of determination means that the independent variable explains more of the dependent variable and this coefficient increases as the number of independent variables increases. In fact, it is somewhat problematic to judge the usefulness of a regression model with only the coefficient of determination because it increases even if a variable that does not explain the dependent variable well is added. 

## Skyline Implementation

### Code

#### R^2

### Logarithm
Log are created to express exponents. For example, 2 to the power of 3 is 8. (2^3=8) And 2 has to be a power of 4 to get 16. (2^4=16) So, what should the power be in order for 2 to equal to 10? A number greater than 3 and less than 4. This number cannot be expressed, it should be expressed it as log_2_10 as a log. That is, log_2_10 becomes an exponent that adds to 2 to make 10. To define x = log_a_b, the exponent that makes a into b is x.

a^x=b -> x=log_a_b

### Conditional Probability
Conditional probability is defined as the likelihood of an event or outcome occurring, based on the occurrence of a previous event or outcome. Conditional probability is calculated by multiplying the probability of the preceding event by the updated probability of the succeeding, or conditional, event. It must be assumed that event A has occurred, so it must be domain a, b. Since event B occurred among these regions a and b, it must be region b. Expressing this as an expression: P(B|A)=P(A∩B)/P(A) 
[logo]: https://mblogthumb-phinf.pstatic.net/20160622_22/alwaysneoi_1466583096349iiYdV_PNG/%C1%B6%B0%C7%BA%CE_%C8%AE%B7%FC.png?type=w2 "Conditional Probability"

### Decision tree
A decision tree is a decision support tool that uses a tree-like model of decisions and their possible consequences, including chance event outcomes, resource costs, and utility. It is one way to display an algorithm that only contains conditional control statements. A decision tree analyzes data and represents a pattern that exists between them as a combination of predictable rules, and is called a decision tree because its shape is like a ‘tree’. It is a concept that narrows the target by asking questions. 

### Entropy
Impurity refers to how many entities of various factors are included. Simply put, it refers to the degree to which several classes are mixed. 

Entropy is a numerical expression of the certainty or amount of information of a probability distribution. Entropy increases when the probabilities of various values appearing as bedbugs are mostly the same. Entropy can also be viewed as one of the characteristic values indicating the shape of the probability distribution. Entropy is said to be low when the probability or probability density is concentrated in a specific value, and conversely, entropy is said to be large when it is spread evenly across various values. The formula for entropy is the equation below.

E(S)=∑^c Pi*I(xi)]

S=collection of events that have already occurred, c=number of events

Amount of information-I(x)=log_2_1/P(x)

Max: when the impurity is the highest, the E(s) is the maximum. 

The smaller the impurity, the purer classification is possible. 

This means that the lower the entropy, the higher the condition must be.

Calculate entropy after division for each feature

IG(S, A) = E(S)-E(S|A)

#### Code

##### Solution

#### Data Tree 

When the dataset is partitioned with the No Diseases property, the information gain is greatest, so we start the tree with no disease.
Accordingly, the root node is assigned No Diseases. When No Diseases is False, the Tree Health is all Poor
Since it is a value, the terminal node is set. If No Diseases is True, entropy and information gain calculations are repeated again.
If you grow the tree with ID3, the above value comes out.

### Range Skline Query 
Range skyline inquiry generalizes point-based dynamic skyline inquiry to search for a dynamic skyline for all individual lookup points in the range. A wide range of applications allows users to submit preferences for a single search value, not limited to submitting preferences for a single search value, but within the interval of 'ideally pursued' values at all levels. The technical contribution of this paper is to introduce and formulate dynamic range skyline queries as a new dominant way to evaluate multidimensional data using range skyline operators. We propose a gradual algorithm using several interesting attributes and pruning strategies to efficiently process the above query in n.r.t. and i.r.t., two types of query predicated parallel to the axis of n-d space. For the spatial axis, we propose an isometric segment of i.r.t. Experimentally verify that the proposed algorithm is I/O optimal and robust in practical terms. 

Let S be an n-d space and P be a dataset of points for S. Q is called a query area. When Q is reduced to a single point, the query represents a calculation that is a dynamic skyline query i.r.t. single query point. The dynamic skyline of the P.i.r.t. query point q(q1, ..., qn) can be calculated as a static skyline query of P after projecting all data points in the original space into the new dynamic data space where q is the origin. The Euclidean distance to q in all dimensions is used as a mapping function of data points. Thus, all data points p in the original space will be projected onto the point p′ (|q1 - p1 |, ..., |qn – pn|). The query predicate Ω may be a hyper right angle iso-angle to the axis of the n-d space because it represents the user's preference composed of intervals of values in all dimensions.

### R-Tree
R-Tree (Rectangle-Tree) is a type of search tree. Like KDB-Tree, R-Tree is a type of data structure extended to enable multi-dimensional search in B-Tree. R-tree divides the space into minimum bounding rectangles and stores them. The minimum bounding rectangles can overlap each other, and the minimum bounding rectangle of the upper level is a Hierarchical Tree Structure including the minimum bounding rectangle of the lower level. In R-Tree, like B-Tree, the size of one node is configured enough to contain one page on the disk.

### Time Complexity of List and Binary Search Tree
Binary search performs a search with the elements sorted and split in half using the sorted attribute. Therefore, there is a characteristic of a sharp decrease in the number of searches. This means that a binary search tree must have the same elements in an ordered form, split in half and have a searchable structure.

List is a data structure that benefits from queries. So, assuming you're only doing searches, you don't need a tree structure. However, assuming that elements can be inserted/deleted, in the list data structure, after finding the index to be inserted/deleted, there is a wasteful process of moving all elements located after the index back one space. Also, increasing the size of an array because there is insufficient space on the array or reducing the size of an array because there is too much space may incur additional time.

The tree structure, on the other hand, has the advantage of not having to move a large amount of elements and not having to worry about space complexity because only the reference needs to be changed. So even if there is only one insert/delete operation, you can insert n times in a row, so you don't need to use the list data structure.

As I said at the beginning, a binary search tree is characterized by not searching all elements. The worst case can be seen as a case of searching as much as the height of the tree (O(n)). So the time complexity of search/insert for height n is O(n). However, time complexity is a slightly better expression when expressed in terms of the number of elements. If H is expressed as the number of elements N , if the number of elements is N , it can be substituted with log_2_N . Therefore, the time complexity of the search/insert operation can be expressed as O(log_2_N).

##############################################################

import random

poiCnt = 300
domainCnt = 8
domainRange = 300

def generatePOI(poiN, domainN, domainR):
  poiDict = dict.fromkeys(range(poiN), 0)
  for i in poiDict:
    poiDict[i]= random.sample(range(domainR),domainN)
  return poiDict

def generateFlagedPOI(origin):
  poiDict = dict()
  for i in origin:
    poiDict[i] = origin[i][:]
    poiDict[i].append([0])
  return poiDict

dictPoi = generatePOI(poiCnt, domainCnt, domainRange)
#dictPoi = {0: [4, 98], 1: [3, 68], 2: [10, 56], 3: [46, 42], 4: [93, 41], 5: [56, 0], 6: [65, 84], 7: [51, 28], 8: [15, 93], 9: [40, 69]}
dictFlagedPoi = generateFlagedPOI(dictPoi)
#dictFlagedPoi

def skylineBruteForce(data, domainN):
  skyline = list()
  for d in data:
    for dCompare in data:
      if data[d][0] > data[dCompare][0] and data[d][1] > data[dCompare][1]and data[d][2] > data[dCompare][2]and data[d][3] > data[dCompare][3]and data[d][4] > data[dCompare][4]:
        data[d][8][0]  = 1
  for d in data:
    if data[d][8][0] == 0:
      skyline.append(d)
  return skyline

def skylineBaseline(data, domainN):
  skyline  = list(data.keys()).copy()
  for k in data.keys():
    for compareK in data.keys():
      if data[k][0] > data[compareK][0]:
        tempCnt = 1
        flag = 1
        while tempCnt<domainN:
          if data[k][tempCnt] <= data[compareK][tempCnt]:
            flag = 0
            break
          tempCnt += 1
        if (flag == 1) and (k in skyline):
           skyline.remove(k)
           break
  return skyline

print("LayerBF: ", skylineLayerBF(dictFlagedPoi, domainCnt))

import time

print("Data: ", dictPoi)
startBf = time.time()
print("BF: ", skylineBruteForce(dictFlagedPoi, domainCnt))
startBL = time.time()
print("BL: ",  skylineBaseline(dictPoi, domainCnt))
endBL = time.time()

print(startBL - startBf, endBL - startBL)

##############################################################
