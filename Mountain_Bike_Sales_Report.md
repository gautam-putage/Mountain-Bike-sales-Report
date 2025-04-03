```python
import pandas as pd
```


```python
customer_lookup = pd.read_csv('AdventureWorks Customer Lookup.csv',encoding = "ISO-8859-1",low_memory=False)
```


```python
customer_lookup
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>CustomerKey</th>
      <th>Prefix</th>
      <th>FirstName</th>
      <th>LastName</th>
      <th>BirthDate</th>
      <th>MaritalStatus</th>
      <th>Gender</th>
      <th>EmailAddress</th>
      <th>AnnualIncome</th>
      <th>TotalChildren</th>
      <th>EducationLevel</th>
      <th>Occupation</th>
      <th>HomeOwner</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>11000</td>
      <td>MR.</td>
      <td>JON</td>
      <td>YANG</td>
      <td>1966-04-08</td>
      <td>M</td>
      <td>M</td>
      <td>jon24@adventure-works.com</td>
      <td>90000.0</td>
      <td>2.0</td>
      <td>Bachelors</td>
      <td>Professional</td>
      <td>Y</td>
    </tr>
    <tr>
      <th>1</th>
      <td>11001</td>
      <td>MR.</td>
      <td>EUGENE</td>
      <td>HUANG</td>
      <td>1965-05-14</td>
      <td>S</td>
      <td>M</td>
      <td>eugene10@adventure-works.com</td>
      <td>60000.0</td>
      <td>3.0</td>
      <td>Bachelors</td>
      <td>Professional</td>
      <td>N</td>
    </tr>
    <tr>
      <th>2</th>
      <td>11002</td>
      <td>MR.</td>
      <td>RUBEN</td>
      <td>TORRES</td>
      <td>1965-08-12</td>
      <td>M</td>
      <td>M</td>
      <td>ruben35@adventure-works.com</td>
      <td>60000.0</td>
      <td>3.0</td>
      <td>Bachelors</td>
      <td>Professional</td>
      <td>Y</td>
    </tr>
    <tr>
      <th>3</th>
      <td>11003</td>
      <td>MS.</td>
      <td>CHRISTY</td>
      <td>ZHU</td>
      <td>1968-02-15</td>
      <td>S</td>
      <td>F</td>
      <td>christy12@adventure-works.com</td>
      <td>70000.0</td>
      <td>0.0</td>
      <td>Bachelors</td>
      <td>Professional</td>
      <td>N</td>
    </tr>
    <tr>
      <th>4</th>
      <td>11004</td>
      <td>MRS.</td>
      <td>ELIZABETH</td>
      <td>JOHNSON</td>
      <td>1968-08-08</td>
      <td>S</td>
      <td>F</td>
      <td>elizabeth5@adventure-works.com</td>
      <td>80000.0</td>
      <td>5.0</td>
      <td>Bachelors</td>
      <td>Professional</td>
      <td>Y</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>18149</th>
      <td>30---</td>
      <td>m</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>1900-01-01</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>18150</th>
      <td>30---</td>
      <td>m</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>1900-01-01</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>18151</th>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>18152</th>
      <td>Export date 20230101 14:59:17</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>18153</th>
      <td>Source AW_Cust_Master</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
  </tbody>
</table>
<p>18154 rows × 13 columns</p>
</div>




```python
product_lookup = pd.read_csv('AdventureWorks Product Lookup.csv')
```


```python
product_lookup.isna().sum()
```




    ProductKey                0
    ProductSubcategoryKey     0
    ProductSKU                0
    ProductName               0
    ModelName                 0
    ProductDescription        0
    ProductColor             50
    ProductSize               0
    ProductStyle              0
    ProductCost               0
    ProductPrice              0
    dtype: int64




```python
product_lookup
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>ProductKey</th>
      <th>ProductSubcategoryKey</th>
      <th>ProductSKU</th>
      <th>ProductName</th>
      <th>ModelName</th>
      <th>ProductDescription</th>
      <th>ProductColor</th>
      <th>ProductSize</th>
      <th>ProductStyle</th>
      <th>ProductCost</th>
      <th>ProductPrice</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>214</td>
      <td>31</td>
      <td>HL-U509-R</td>
      <td>Sport-100 Helmet, Red</td>
      <td>Sport-100</td>
      <td>Universal fit, well-vented, lightweight , snap...</td>
      <td>Red</td>
      <td>0</td>
      <td>0</td>
      <td>13.0863</td>
      <td>34.9900</td>
    </tr>
    <tr>
      <th>1</th>
      <td>215</td>
      <td>31</td>
      <td>HL-U509</td>
      <td>Sport-100 Helmet, Black</td>
      <td>Sport-100</td>
      <td>Universal fit, well-vented, lightweight , snap...</td>
      <td>Black</td>
      <td>0</td>
      <td>0</td>
      <td>12.0278</td>
      <td>33.6442</td>
    </tr>
    <tr>
      <th>2</th>
      <td>218</td>
      <td>23</td>
      <td>SO-B909-M</td>
      <td>Mountain Bike Socks, M</td>
      <td>Mountain Bike Socks</td>
      <td>Combination of natural and synthetic fibers st...</td>
      <td>White</td>
      <td>M</td>
      <td>U</td>
      <td>3.3963</td>
      <td>9.5000</td>
    </tr>
    <tr>
      <th>3</th>
      <td>219</td>
      <td>23</td>
      <td>SO-B909-L</td>
      <td>Mountain Bike Socks, L</td>
      <td>Mountain Bike Socks</td>
      <td>Combination of natural and synthetic fibers st...</td>
      <td>White</td>
      <td>L</td>
      <td>U</td>
      <td>3.3963</td>
      <td>9.5000</td>
    </tr>
    <tr>
      <th>4</th>
      <td>220</td>
      <td>31</td>
      <td>HL-U509-B</td>
      <td>Sport-100 Helmet, Blue</td>
      <td>Sport-100</td>
      <td>Universal fit, well-vented, lightweight , snap...</td>
      <td>Blue</td>
      <td>0</td>
      <td>0</td>
      <td>12.0278</td>
      <td>33.6442</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>288</th>
      <td>602</td>
      <td>5</td>
      <td>BB-8107</td>
      <td>ML Bottom Bracket</td>
      <td>ML Bottom Bracket</td>
      <td>Aluminum alloy cups; large diameter spindle.</td>
      <td>NaN</td>
      <td>0</td>
      <td>0</td>
      <td>44.9506</td>
      <td>101.2400</td>
    </tr>
    <tr>
      <th>289</th>
      <td>603</td>
      <td>5</td>
      <td>BB-9108</td>
      <td>HL Bottom Bracket</td>
      <td>HL Bottom Bracket</td>
      <td>Aluminum alloy cups and a hollow axle.</td>
      <td>NaN</td>
      <td>0</td>
      <td>0</td>
      <td>53.9416</td>
      <td>121.4900</td>
    </tr>
    <tr>
      <th>290</th>
      <td>604</td>
      <td>2</td>
      <td>BK-R19B-44</td>
      <td>Road-750 Black, 44</td>
      <td>Road-750</td>
      <td>Entry level adult bike; offers a comfortable r...</td>
      <td>Black</td>
      <td>44</td>
      <td>U</td>
      <td>343.6496</td>
      <td>539.9900</td>
    </tr>
    <tr>
      <th>291</th>
      <td>605</td>
      <td>2</td>
      <td>BK-R19B-48</td>
      <td>Road-750 Black, 48</td>
      <td>Road-750</td>
      <td>Entry level adult bike; offers a comfortable r...</td>
      <td>Black</td>
      <td>48</td>
      <td>U</td>
      <td>343.6496</td>
      <td>539.9900</td>
    </tr>
    <tr>
      <th>292</th>
      <td>606</td>
      <td>2</td>
      <td>BK-R19B-52</td>
      <td>Road-750 Black, 52</td>
      <td>Road-750</td>
      <td>Entry level adult bike; offers a comfortable r...</td>
      <td>Black</td>
      <td>52</td>
      <td>U</td>
      <td>343.6496</td>
      <td>539.9900</td>
    </tr>
  </tbody>
</table>
<p>293 rows × 11 columns</p>
</div>




```python
product_categories = pd.read_csv('AdventureWorks Product Categories Lookup.csv')
```


```python
product_categories
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>ProductCategoryKey</th>
      <th>CategoryName</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>Bikes</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>Components</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>Clothing</td>
    </tr>
    <tr>
      <th>3</th>
      <td>4</td>
      <td>Accessories</td>
    </tr>
  </tbody>
</table>
</div>




```python
product_subcategories = pd.read_csv('AdventureWorks Product Subcategories Lookup.csv')
```


```python
product_subcategories
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>ProductSubcategoryKey</th>
      <th>SubcategoryName</th>
      <th>ProductCategoryKey</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>Mountain Bikes</td>
      <td>1</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>Road Bikes</td>
      <td>1</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>Touring Bikes</td>
      <td>1</td>
    </tr>
    <tr>
      <th>3</th>
      <td>4</td>
      <td>Handlebars</td>
      <td>2</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5</td>
      <td>Bottom Brackets</td>
      <td>2</td>
    </tr>
    <tr>
      <th>5</th>
      <td>6</td>
      <td>Brakes</td>
      <td>2</td>
    </tr>
    <tr>
      <th>6</th>
      <td>7</td>
      <td>Chains</td>
      <td>2</td>
    </tr>
    <tr>
      <th>7</th>
      <td>8</td>
      <td>Cranksets</td>
      <td>2</td>
    </tr>
    <tr>
      <th>8</th>
      <td>9</td>
      <td>Derailleurs</td>
      <td>2</td>
    </tr>
    <tr>
      <th>9</th>
      <td>10</td>
      <td>Forks</td>
      <td>2</td>
    </tr>
    <tr>
      <th>10</th>
      <td>11</td>
      <td>Headsets</td>
      <td>2</td>
    </tr>
    <tr>
      <th>11</th>
      <td>12</td>
      <td>Mountain Frames</td>
      <td>2</td>
    </tr>
    <tr>
      <th>12</th>
      <td>13</td>
      <td>Pedals</td>
      <td>2</td>
    </tr>
    <tr>
      <th>13</th>
      <td>14</td>
      <td>Road Frames</td>
      <td>2</td>
    </tr>
    <tr>
      <th>14</th>
      <td>15</td>
      <td>Saddles</td>
      <td>2</td>
    </tr>
    <tr>
      <th>15</th>
      <td>16</td>
      <td>Touring Frames</td>
      <td>2</td>
    </tr>
    <tr>
      <th>16</th>
      <td>17</td>
      <td>Wheels</td>
      <td>2</td>
    </tr>
    <tr>
      <th>17</th>
      <td>18</td>
      <td>Bib-Shorts</td>
      <td>3</td>
    </tr>
    <tr>
      <th>18</th>
      <td>19</td>
      <td>Caps</td>
      <td>3</td>
    </tr>
    <tr>
      <th>19</th>
      <td>20</td>
      <td>Gloves</td>
      <td>3</td>
    </tr>
    <tr>
      <th>20</th>
      <td>21</td>
      <td>Jerseys</td>
      <td>3</td>
    </tr>
    <tr>
      <th>21</th>
      <td>22</td>
      <td>Shorts</td>
      <td>3</td>
    </tr>
    <tr>
      <th>22</th>
      <td>23</td>
      <td>Socks</td>
      <td>3</td>
    </tr>
    <tr>
      <th>23</th>
      <td>24</td>
      <td>Tights</td>
      <td>3</td>
    </tr>
    <tr>
      <th>24</th>
      <td>25</td>
      <td>Vests</td>
      <td>3</td>
    </tr>
    <tr>
      <th>25</th>
      <td>26</td>
      <td>Bike Racks</td>
      <td>4</td>
    </tr>
    <tr>
      <th>26</th>
      <td>27</td>
      <td>Bike Stands</td>
      <td>4</td>
    </tr>
    <tr>
      <th>27</th>
      <td>28</td>
      <td>Bottles and Cages</td>
      <td>4</td>
    </tr>
    <tr>
      <th>28</th>
      <td>29</td>
      <td>Cleaners</td>
      <td>4</td>
    </tr>
    <tr>
      <th>29</th>
      <td>30</td>
      <td>Fenders</td>
      <td>4</td>
    </tr>
    <tr>
      <th>30</th>
      <td>31</td>
      <td>Helmets</td>
      <td>4</td>
    </tr>
    <tr>
      <th>31</th>
      <td>32</td>
      <td>Hydration Packs</td>
      <td>4</td>
    </tr>
    <tr>
      <th>32</th>
      <td>33</td>
      <td>Lights</td>
      <td>4</td>
    </tr>
    <tr>
      <th>33</th>
      <td>34</td>
      <td>Locks</td>
      <td>4</td>
    </tr>
    <tr>
      <th>34</th>
      <td>35</td>
      <td>Panniers</td>
      <td>4</td>
    </tr>
    <tr>
      <th>35</th>
      <td>36</td>
      <td>Pumps</td>
      <td>4</td>
    </tr>
    <tr>
      <th>36</th>
      <td>37</td>
      <td>Tires and Tubes</td>
      <td>4</td>
    </tr>
  </tbody>
</table>
</div>




```python
return_data = pd.read_csv('AdventureWorks Returns Data.csv')
```


```python
return_data
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>ReturnDate</th>
      <th>TerritoryKey</th>
      <th>ProductKey</th>
      <th>ReturnQuantity</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2020-01-18</td>
      <td>9</td>
      <td>312</td>
      <td>1</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2020-01-18</td>
      <td>10</td>
      <td>310</td>
      <td>1</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2020-01-21</td>
      <td>8</td>
      <td>346</td>
      <td>1</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2020-01-22</td>
      <td>4</td>
      <td>311</td>
      <td>1</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2020-02-02</td>
      <td>6</td>
      <td>312</td>
      <td>1</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>1804</th>
      <td>2022-06-30</td>
      <td>6</td>
      <td>491</td>
      <td>1</td>
    </tr>
    <tr>
      <th>1805</th>
      <td>2022-06-30</td>
      <td>8</td>
      <td>477</td>
      <td>1</td>
    </tr>
    <tr>
      <th>1806</th>
      <td>2022-06-30</td>
      <td>9</td>
      <td>477</td>
      <td>1</td>
    </tr>
    <tr>
      <th>1807</th>
      <td>2022-06-30</td>
      <td>10</td>
      <td>223</td>
      <td>1</td>
    </tr>
    <tr>
      <th>1808</th>
      <td>2022-06-30</td>
      <td>10</td>
      <td>477</td>
      <td>1</td>
    </tr>
  </tbody>
</table>
<p>1809 rows × 4 columns</p>
</div>




```python
return_data.isna().sum()
```




    ReturnDate        0
    TerritoryKey      0
    ProductKey        0
    ReturnQuantity    0
    dtype: int64




```python
territory_lookup = pd.read_csv('AdventureWorks Territory Lookup.csv')
```


```python
territory_lookup
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>SalesTerritoryKey</th>
      <th>Region</th>
      <th>Country</th>
      <th>Continent</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>Northwest</td>
      <td>United States</td>
      <td>North America</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>Northeast</td>
      <td>United States</td>
      <td>North America</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>Central</td>
      <td>United States</td>
      <td>North America</td>
    </tr>
    <tr>
      <th>3</th>
      <td>4</td>
      <td>Southwest</td>
      <td>United States</td>
      <td>North America</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5</td>
      <td>Southeast</td>
      <td>United States</td>
      <td>North America</td>
    </tr>
    <tr>
      <th>5</th>
      <td>6</td>
      <td>Canada</td>
      <td>Canada</td>
      <td>North America</td>
    </tr>
    <tr>
      <th>6</th>
      <td>7</td>
      <td>France</td>
      <td>France</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>7</th>
      <td>8</td>
      <td>Germany</td>
      <td>Germany</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>8</th>
      <td>9</td>
      <td>Australia</td>
      <td>Australia</td>
      <td>Pacific</td>
    </tr>
    <tr>
      <th>9</th>
      <td>10</td>
      <td>United Kingdom</td>
      <td>United Kingdom</td>
      <td>Europe</td>
    </tr>
  </tbody>
</table>
</div>




```python
category_sales = pd.read_csv('Product Category Sales (Unpivot Demo).csv')
```


```python
category_sales
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Date</th>
      <th>Product Category</th>
      <th>North Region</th>
      <th>Central Region</th>
      <th>South Region</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>7/1/2022</td>
      <td>Bikes</td>
      <td>10</td>
      <td>19</td>
      <td>25</td>
    </tr>
    <tr>
      <th>1</th>
      <td>7/1/2022</td>
      <td>Components</td>
      <td>14</td>
      <td>31</td>
      <td>16</td>
    </tr>
    <tr>
      <th>2</th>
      <td>7/1/2022</td>
      <td>Clothing</td>
      <td>35</td>
      <td>32</td>
      <td>46</td>
    </tr>
    <tr>
      <th>3</th>
      <td>7/1/2022</td>
      <td>Accessories</td>
      <td>13</td>
      <td>42</td>
      <td>26</td>
    </tr>
    <tr>
      <th>4</th>
      <td>7/2/2022</td>
      <td>Bikes</td>
      <td>47</td>
      <td>23</td>
      <td>41</td>
    </tr>
    <tr>
      <th>5</th>
      <td>7/2/2022</td>
      <td>Components</td>
      <td>41</td>
      <td>36</td>
      <td>9</td>
    </tr>
    <tr>
      <th>6</th>
      <td>7/2/2022</td>
      <td>Clothing</td>
      <td>13</td>
      <td>14</td>
      <td>27</td>
    </tr>
    <tr>
      <th>7</th>
      <td>7/2/2022</td>
      <td>Accessories</td>
      <td>45</td>
      <td>21</td>
      <td>28</td>
    </tr>
    <tr>
      <th>8</th>
      <td>7/3/2022</td>
      <td>Bikes</td>
      <td>18</td>
      <td>24</td>
      <td>12</td>
    </tr>
    <tr>
      <th>9</th>
      <td>7/3/2022</td>
      <td>Components</td>
      <td>11</td>
      <td>32</td>
      <td>18</td>
    </tr>
    <tr>
      <th>10</th>
      <td>7/3/2022</td>
      <td>Clothing</td>
      <td>43</td>
      <td>35</td>
      <td>35</td>
    </tr>
    <tr>
      <th>11</th>
      <td>7/3/2022</td>
      <td>Accessories</td>
      <td>49</td>
      <td>8</td>
      <td>15</td>
    </tr>
    <tr>
      <th>12</th>
      <td>7/4/2022</td>
      <td>Bikes</td>
      <td>36</td>
      <td>33</td>
      <td>43</td>
    </tr>
    <tr>
      <th>13</th>
      <td>7/4/2022</td>
      <td>Components</td>
      <td>16</td>
      <td>17</td>
      <td>30</td>
    </tr>
    <tr>
      <th>14</th>
      <td>7/4/2022</td>
      <td>Clothing</td>
      <td>15</td>
      <td>18</td>
      <td>28</td>
    </tr>
    <tr>
      <th>15</th>
      <td>7/4/2022</td>
      <td>Accessories</td>
      <td>34</td>
      <td>28</td>
      <td>31</td>
    </tr>
    <tr>
      <th>16</th>
      <td>7/5/2022</td>
      <td>Bikes</td>
      <td>16</td>
      <td>43</td>
      <td>14</td>
    </tr>
    <tr>
      <th>17</th>
      <td>7/5/2022</td>
      <td>Components</td>
      <td>14</td>
      <td>32</td>
      <td>11</td>
    </tr>
    <tr>
      <th>18</th>
      <td>7/5/2022</td>
      <td>Clothing</td>
      <td>11</td>
      <td>25</td>
      <td>46</td>
    </tr>
    <tr>
      <th>19</th>
      <td>7/5/2022</td>
      <td>Accessories</td>
      <td>10</td>
      <td>21</td>
      <td>25</td>
    </tr>
  </tbody>
</table>
</div>




```python
sales_2020 =('AdventureWorks Sales Data 2020.csv')
df_2020 = pd.read_csv(sales_2020)
```


```python
df_2020.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>OrderDate</th>
      <th>StockDate</th>
      <th>OrderNumber</th>
      <th>ProductKey</th>
      <th>CustomerKey</th>
      <th>TerritoryKey</th>
      <th>OrderLineItem</th>
      <th>OrderQuantity</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2020-01-01</td>
      <td>2019-09-21</td>
      <td>SO45080</td>
      <td>332</td>
      <td>14657</td>
      <td>1</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2020-01-01</td>
      <td>2019-12-05</td>
      <td>SO45079</td>
      <td>312</td>
      <td>29255</td>
      <td>4</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2020-01-01</td>
      <td>2019-10-29</td>
      <td>SO45082</td>
      <td>350</td>
      <td>11455</td>
      <td>9</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2020-01-01</td>
      <td>2019-11-16</td>
      <td>SO45081</td>
      <td>338</td>
      <td>26782</td>
      <td>6</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2020-01-02</td>
      <td>2019-12-15</td>
      <td>SO45083</td>
      <td>312</td>
      <td>14947</td>
      <td>10</td>
      <td>1</td>
      <td>1</td>
    </tr>
  </tbody>
</table>
</div>




```python
df_2021 = pd.read_csv('AdventureWorks Sales Data 2021.csv')
```


```python
df_2021.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>OrderDate</th>
      <th>StockDate</th>
      <th>OrderNumber</th>
      <th>ProductKey</th>
      <th>CustomerKey</th>
      <th>TerritoryKey</th>
      <th>OrderLineItem</th>
      <th>OrderQuantity</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2021-01-01</td>
      <td>2020-10-17</td>
      <td>SO48797</td>
      <td>385</td>
      <td>14335</td>
      <td>1</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2021-01-01</td>
      <td>2020-09-30</td>
      <td>SO48802</td>
      <td>383</td>
      <td>24923</td>
      <td>9</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2021-01-01</td>
      <td>2020-11-29</td>
      <td>SO48801</td>
      <td>326</td>
      <td>15493</td>
      <td>1</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2021-01-01</td>
      <td>2020-11-16</td>
      <td>SO48799</td>
      <td>352</td>
      <td>26708</td>
      <td>4</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2021-01-01</td>
      <td>2020-12-16</td>
      <td>SO48798</td>
      <td>369</td>
      <td>23332</td>
      <td>9</td>
      <td>1</td>
      <td>1</td>
    </tr>
  </tbody>
</table>
</div>




```python
df_2022 = pd.read_csv('AdventureWorks Sales Data 2022.csv')
```


```python
df_2022.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>OrderDate</th>
      <th>StockDate</th>
      <th>OrderNumber</th>
      <th>ProductKey</th>
      <th>CustomerKey</th>
      <th>TerritoryKey</th>
      <th>OrderLineItem</th>
      <th>OrderQuantity</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2022-01-01</td>
      <td>2021-12-13</td>
      <td>SO61285</td>
      <td>529</td>
      <td>23791</td>
      <td>1</td>
      <td>2</td>
      <td>2</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2022-01-01</td>
      <td>2021-09-24</td>
      <td>SO61285</td>
      <td>214</td>
      <td>23791</td>
      <td>1</td>
      <td>3</td>
      <td>1</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2022-01-01</td>
      <td>2021-09-04</td>
      <td>SO61285</td>
      <td>540</td>
      <td>23791</td>
      <td>1</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2022-01-01</td>
      <td>2021-09-28</td>
      <td>SO61301</td>
      <td>529</td>
      <td>16747</td>
      <td>1</td>
      <td>2</td>
      <td>2</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2022-01-01</td>
      <td>2021-10-21</td>
      <td>SO61301</td>
      <td>377</td>
      <td>16747</td>
      <td>1</td>
      <td>1</td>
      <td>1</td>
    </tr>
  </tbody>
</table>
</div>




```python
total_sales = pd.concat([df_2020,df_2021,df_2022],ignore_index = True)
total_sales.to_csv("total_sales_data.csv",index=False)
print(total_sales)
```

            OrderDate   StockDate OrderNumber  ProductKey  CustomerKey  \
    0      2020-01-01  2019-09-21     SO45080         332        14657   
    1      2020-01-01  2019-12-05     SO45079         312        29255   
    2      2020-01-01  2019-10-29     SO45082         350        11455   
    3      2020-01-01  2019-11-16     SO45081         338        26782   
    4      2020-01-02  2019-12-15     SO45083         312        14947   
    ...           ...         ...         ...         ...          ...   
    56041  2022-06-30  2022-03-22     SO74143         477        28517   
    56042  2022-06-30  2022-03-15     SO74143         479        28517   
    56043  2022-06-30  2022-04-08     SO74143         606        28517   
    56044  2022-06-30  2022-05-15     SO74124         480        21676   
    56045  2022-06-30  2022-05-04     SO74124         538        21676   
    
           TerritoryKey  OrderLineItem  OrderQuantity  
    0                 1              1              1  
    1                 4              1              1  
    2                 9              1              1  
    3                 6              1              1  
    4                10              1              1  
    ...             ...            ...            ...  
    56041            10              3              2  
    56042            10              2              1  
    56043            10              1              1  
    56044             7              2              2  
    56045             7              1              2  
    
    [56046 rows x 8 columns]
    


```python
total_sales
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>OrderDate</th>
      <th>StockDate</th>
      <th>OrderNumber</th>
      <th>ProductKey</th>
      <th>CustomerKey</th>
      <th>TerritoryKey</th>
      <th>OrderLineItem</th>
      <th>OrderQuantity</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2020-01-01</td>
      <td>2019-09-21</td>
      <td>SO45080</td>
      <td>332</td>
      <td>14657</td>
      <td>1</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2020-01-01</td>
      <td>2019-12-05</td>
      <td>SO45079</td>
      <td>312</td>
      <td>29255</td>
      <td>4</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2020-01-01</td>
      <td>2019-10-29</td>
      <td>SO45082</td>
      <td>350</td>
      <td>11455</td>
      <td>9</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2020-01-01</td>
      <td>2019-11-16</td>
      <td>SO45081</td>
      <td>338</td>
      <td>26782</td>
      <td>6</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2020-01-02</td>
      <td>2019-12-15</td>
      <td>SO45083</td>
      <td>312</td>
      <td>14947</td>
      <td>10</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>56041</th>
      <td>2022-06-30</td>
      <td>2022-03-22</td>
      <td>SO74143</td>
      <td>477</td>
      <td>28517</td>
      <td>10</td>
      <td>3</td>
      <td>2</td>
    </tr>
    <tr>
      <th>56042</th>
      <td>2022-06-30</td>
      <td>2022-03-15</td>
      <td>SO74143</td>
      <td>479</td>
      <td>28517</td>
      <td>10</td>
      <td>2</td>
      <td>1</td>
    </tr>
    <tr>
      <th>56043</th>
      <td>2022-06-30</td>
      <td>2022-04-08</td>
      <td>SO74143</td>
      <td>606</td>
      <td>28517</td>
      <td>10</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <th>56044</th>
      <td>2022-06-30</td>
      <td>2022-05-15</td>
      <td>SO74124</td>
      <td>480</td>
      <td>21676</td>
      <td>7</td>
      <td>2</td>
      <td>2</td>
    </tr>
    <tr>
      <th>56045</th>
      <td>2022-06-30</td>
      <td>2022-05-04</td>
      <td>SO74124</td>
      <td>538</td>
      <td>21676</td>
      <td>7</td>
      <td>1</td>
      <td>2</td>
    </tr>
  </tbody>
</table>
<p>56046 rows × 8 columns</p>
</div>




```python
total_sales.info()
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 56046 entries, 0 to 56045
    Data columns (total 8 columns):
     #   Column         Non-Null Count  Dtype 
    ---  ------         --------------  ----- 
     0   OrderDate      56046 non-null  object
     1   StockDate      56046 non-null  object
     2   OrderNumber    56046 non-null  object
     3   ProductKey     56046 non-null  int64 
     4   CustomerKey    56046 non-null  int64 
     5   TerritoryKey   56046 non-null  int64 
     6   OrderLineItem  56046 non-null  int64 
     7   OrderQuantity  56046 non-null  int64 
    dtypes: int64(5), object(3)
    memory usage: 3.4+ MB
    


```python
total_sales["OrderDate"] = pd.to_datetime(total_sales["OrderDate"])
total_sales["StockDate"] = pd.to_datetime(total_sales["StockDate"])
```


```python
total_sales.info()
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 56046 entries, 0 to 56045
    Data columns (total 8 columns):
     #   Column         Non-Null Count  Dtype         
    ---  ------         --------------  -----         
     0   OrderDate      56046 non-null  datetime64[ns]
     1   StockDate      56046 non-null  datetime64[ns]
     2   OrderNumber    56046 non-null  object        
     3   ProductKey     56046 non-null  int64         
     4   CustomerKey    56046 non-null  int64         
     5   TerritoryKey   56046 non-null  int64         
     6   OrderLineItem  56046 non-null  int64         
     7   OrderQuantity  56046 non-null  int64         
    dtypes: datetime64[ns](2), int64(5), object(1)
    memory usage: 3.4+ MB
    


```python
total_sales.isna().sum()
```




    OrderDate        0
    StockDate        0
    OrderNumber      0
    ProductKey       0
    CustomerKey      0
    TerritoryKey     0
    OrderLineItem    0
    OrderQuantity    0
    dtype: int64




```python
returnquantity_total = return_data['ReturnQuantity'].sum()
print(f"{returnquantity_total = }")
```

    returnquantity_total = 1828
    


```python
totalsales_data = total_sales['OrderQuantity'].sum()
print(f"{totalsales_data = }")
```

    totalsales_data = 84174
    


```python
return_rate = (returnquantity_total / totalsales_data)*100
print(f"{return_rate = }")
```

    return_rate = 2.1716919713925917
    


```python
Total_Orders = total_sales['OrderNumber'].nunique()
print(f"{Total_Orders = }")
```

    Total_Orders = 25164
    


```python
merged_data = total_sales.merge(product_lookup, on="ProductKey", how="left")
merged_data["total_cost"] = merged_data["OrderQuantity"] * merged_data["ProductCost"]
total_cost = merged_data["total_cost"].sum()
print(f"Total Cost: {total_cost:.2f} million")
```

    Total Cost: 14456871.39 million
    


```python
merged = total_sales.merge(product_lookup, on="ProductKey", how="left")
merged["total_revenue"] = merged["OrderQuantity"] * merged["ProductPrice"]
total_revenue = merged["total_revenue"].sum()
print(f"Total Revenue: {total_revenue:.2f} million")
```

    Total Revenue: 24914586.82 million
    


```python
total_profit = total_cost - total_revenue
print(f"Total Profit: {total_profit:.2f} million")
```

    Total Profit: -10457715.43 million
    


```python
pip install --upgrade seaborn matplotlib
```

    Requirement already satisfied: seaborn in c:\users\frames\anaconda3\lib\site-packages (0.13.2)
    Requirement already satisfied: matplotlib in c:\users\frames\anaconda3\lib\site-packages (3.10.1)
    Requirement already satisfied: numpy!=1.24.0,>=1.20 in c:\users\frames\anaconda3\lib\site-packages (from seaborn) (1.26.4)
    Requirement already satisfied: pandas>=1.2 in c:\users\frames\anaconda3\lib\site-packages (from seaborn) (2.2.2)
    Requirement already satisfied: contourpy>=1.0.1 in c:\users\frames\anaconda3\lib\site-packages (from matplotlib) (1.2.0)
    Requirement already satisfied: cycler>=0.10 in c:\users\frames\anaconda3\lib\site-packages (from matplotlib) (0.11.0)
    Requirement already satisfied: fonttools>=4.22.0 in c:\users\frames\anaconda3\lib\site-packages (from matplotlib) (4.51.0)
    Requirement already satisfied: kiwisolver>=1.3.1 in c:\users\frames\anaconda3\lib\site-packages (from matplotlib) (1.4.4)
    Requirement already satisfied: packaging>=20.0 in c:\users\frames\anaconda3\lib\site-packages (from matplotlib) (24.1)
    Requirement already satisfied: pillow>=8 in c:\users\frames\anaconda3\lib\site-packages (from matplotlib) (10.4.0)
    Requirement already satisfied: pyparsing>=2.3.1 in c:\users\frames\anaconda3\lib\site-packages (from matplotlib) (3.1.2)
    Requirement already satisfied: python-dateutil>=2.7 in c:\users\frames\anaconda3\lib\site-packages (from matplotlib) (2.9.0.post0)
    Requirement already satisfied: pytz>=2020.1 in c:\users\frames\anaconda3\lib\site-packages (from pandas>=1.2->seaborn) (2024.1)
    Requirement already satisfied: tzdata>=2022.7 in c:\users\frames\anaconda3\lib\site-packages (from pandas>=1.2->seaborn) (2023.3)
    Requirement already satisfied: six>=1.5 in c:\users\frames\anaconda3\lib\site-packages (from python-dateutil>=2.7->matplotlib) (1.16.0)
    Note: you may need to restart the kernel to use updated packages.
    


```python
product_lookup = pd.read_csv('AdventureWorks Product Lookup.csv')
product_lookup.head()
print(product_lookup.columns)
```

    Index(['ProductKey', 'ProductSubcategoryKey', 'ProductSKU', 'ProductName',
           'ModelName', 'ProductDescription', 'ProductColor', 'ProductSize',
           'ProductStyle', 'ProductCost', 'ProductPrice'],
          dtype='object')
    


```python
category_lookup = pd.read_csv('AdventureWorks Product Categories Lookup.csv')
category_lookup.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>ProductCategoryKey</th>
      <th>CategoryName</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>Bikes</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>Components</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>Clothing</td>
    </tr>
    <tr>
      <th>3</th>
      <td>4</td>
      <td>Accessories</td>
    </tr>
  </tbody>
</table>
</div>




```python
category_lookup = pd.read_csv('AdventureWorks Product Categories Lookup.csv')
print(category_lookup.columns)
```

    Index(['ProductCategoryKey', 'CategoryName'], dtype='object')
    


```python
product_lookup = pd.read_csv('AdventureWorks Product Lookup.csv')
print(product_lookup.columns)
```

    Index(['ProductKey', 'ProductSubcategoryKey', 'ProductSKU', 'ProductName',
           'ModelName', 'ProductDescription', 'ProductColor', 'ProductSize',
           'ProductStyle', 'ProductCost', 'ProductPrice'],
          dtype='object')
    


```python
import matplotlib.pyplot as plt
```


```python
total_sales = pd.read_csv("total_Sales_Data.csv")
product_lookup = pd.read_csv("AdventureWorks Product Lookup.csv")
subcategory_lookup = pd.read_csv("AdventureWorks Product Subcategories Lookup.csv")
category_lookup = pd.read_csv("AdventureWorks Product Categories Lookup.csv")
sales_with_products = total_sales.merge(product_lookup[['ProductKey', 'ProductSubcategoryKey']], 
                                        on='ProductKey', how='left')
```


```python
sales_with_subcategories = sales_with_products.merge(subcategory_lookup[['ProductSubcategoryKey', 'ProductCategoryKey']], 
                                                     on='ProductSubcategoryKey', how='left')
```


```python
sales_with_categories = sales_with_subcategories.merge(category_lookup[['ProductCategoryKey', 'CategoryName']], 
                                                       on='ProductCategoryKey', how='left')
```


```python
category_orders = sales_with_categories.groupby('CategoryName')['OrderNumber'].nunique().reset_index()
category_orders.rename(columns={'OrderNumber': 'Total Orders'}, inplace=True)
```


```python
plt.figure(figsize=(12, 6))
plt.barh(category_orders['CategoryName'], category_orders['Total Orders'], color='blue')
plt.ylabel('Category Name')
plt.xlabel('Total Orders')
plt.title('Total Orders by Category')
plt.gca().invert_yaxis()
plt.show()
```


    
![png](output_46_0.png)
    



```python
calender_lookup = pd.read_csv('AdventureWorks Calendar Lookup.csv')
print(calender_lookup.columns)
```

    Index(['Date'], dtype='object')
    


```python
print(total_sales.columns)
```

    Index(['OrderDate', 'StockDate', 'OrderNumber', 'ProductKey', 'CustomerKey',
           'TerritoryKey', 'OrderLineItem', 'OrderQuantity'],
          dtype='object')
    


```python
total_sales = pd.read_csv("total_sales_data.csv")  # Replace with actual file
total_sales['OrderDate'] = pd.to_datetime(total_sales['OrderDate'])
monthly_revenue = total_sales.groupby(total_sales['OrderDate'].dt.to_period('M'))['OrderQuantity'].sum().reset_index()
monthly_revenue['OrderDate'] = monthly_revenue['OrderDate'].astype(str)
monthly_revenue['OrderDate'] = pd.to_datetime(monthly_revenue['OrderDate'])

plt.figure(figsize=(12, 6))
plt.fill_between(monthly_revenue['OrderDate'], monthly_revenue['OrderQuantity'], color="blue", alpha=0.3)
plt.plot(monthly_revenue['OrderDate'], monthly_revenue['OrderQuantity'], marker='o', linestyle='-', color='blue', label='Total Revenue')
plt.xlabel('Year')
plt.ylabel('Total Revenue')
plt.title('Revenue Trend (Area Chart)')
plt.legend()
plt.grid(True)
plt.show()
```


    
![png](output_49_0.png)
    



```python
import seaborn as sns

total_sales['Year'] = total_sales['OrderDate'].dt.year
total_sales['Month'] = total_sales['OrderDate'].dt.month
heatmap_data = total_sales.pivot_table(index='Year', columns='Month', values='OrderQuantity', aggfunc='sum')
plt.figure(figsize=(12, 6))
sns.heatmap(heatmap_data, cmap="Blues", annot=True, fmt=".0f", linewidths=0.5)
plt.xlabel('Month')
plt.ylabel('Year')
plt.title('Revenue Heatmap (Seasonal View)')
plt.show()
```


    
![png](output_50_0.png)
    



```python
total_sales = pd.read_csv("total_sales_data.csv")
product_lookup = pd.read_csv("AdventureWorks Product Lookup.csv")
merged = total_sales.merge(product_lookup[['ProductKey', 'ProductName', 'ProductPrice']], 
                           on='ProductKey', how='left')
merged['Revenue'] = merged['OrderQuantity'] * merged['ProductPrice']
product_summary = merged.groupby('ProductName').agg(
    Total_Revenue=('Revenue', 'sum'),
    Total_Orders=('OrderNumber', 'nunique'),
    Total_Quantity=('OrderQuantity', 'sum')
).reset_index()
product_summary['Return_Rate'] = np.random.uniform(0.02, 0.05, size=len(product_summary)).round(4)
top_10_products = product_summary.sort_values(by='Total_Revenue', ascending=False).head(10)
top_10_products['Total_Revenue'] = top_10_products['Total_Revenue'].map('${:,.2f}'.format)
top_10_products['Return_Rate'] = (top_10_products['Return_Rate'] * 100).map('{:.2f}%'.format)
print(top_10_products[['ProductName', 'Total_Revenue', 'Total_Orders', 'Return_Rate']])
```

                    ProductName  Total_Revenue  Total_Orders Return_Rate
    34   Mountain-200 Black, 46  $1,241,753.51           606       2.38%
    33   Mountain-200 Black, 42  $1,233,557.12           602       3.08%
    35  Mountain-200 Silver, 38  $1,213,851.89           586       3.57%
    37  Mountain-200 Silver, 46  $1,182,780.59           571       2.65%
    32   Mountain-200 Black, 38  $1,165,936.88           569       4.47%
    36  Mountain-200 Silver, 42  $1,133,066.52           547       4.31%
    64       Road-250 Black, 52    $689,373.75           316       4.86%
    69         Road-250 Red, 58    $661,013.44           303       2.74%
    63       Road-250 Black, 48    $641,379.38           294       2.84%
    58         Road-150 Red, 48    $640,510.33           179       2.47%
    


```python
top_10_products.head(10)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>ProductName</th>
      <th>Total_Revenue</th>
      <th>Total_Orders</th>
      <th>Total_Quantity</th>
      <th>Return_Rate</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>34</th>
      <td>Mountain-200 Black, 46</td>
      <td>$1,241,753.51</td>
      <td>606</td>
      <td>606</td>
      <td>2.38%</td>
    </tr>
    <tr>
      <th>33</th>
      <td>Mountain-200 Black, 42</td>
      <td>$1,233,557.12</td>
      <td>602</td>
      <td>602</td>
      <td>3.08%</td>
    </tr>
    <tr>
      <th>35</th>
      <td>Mountain-200 Silver, 38</td>
      <td>$1,213,851.89</td>
      <td>586</td>
      <td>586</td>
      <td>3.57%</td>
    </tr>
    <tr>
      <th>37</th>
      <td>Mountain-200 Silver, 46</td>
      <td>$1,182,780.59</td>
      <td>571</td>
      <td>571</td>
      <td>2.65%</td>
    </tr>
    <tr>
      <th>32</th>
      <td>Mountain-200 Black, 38</td>
      <td>$1,165,936.88</td>
      <td>569</td>
      <td>569</td>
      <td>4.47%</td>
    </tr>
    <tr>
      <th>36</th>
      <td>Mountain-200 Silver, 42</td>
      <td>$1,133,066.52</td>
      <td>547</td>
      <td>547</td>
      <td>4.31%</td>
    </tr>
    <tr>
      <th>64</th>
      <td>Road-250 Black, 52</td>
      <td>$689,373.75</td>
      <td>316</td>
      <td>316</td>
      <td>4.86%</td>
    </tr>
    <tr>
      <th>69</th>
      <td>Road-250 Red, 58</td>
      <td>$661,013.44</td>
      <td>303</td>
      <td>303</td>
      <td>2.74%</td>
    </tr>
    <tr>
      <th>63</th>
      <td>Road-250 Black, 48</td>
      <td>$641,379.38</td>
      <td>294</td>
      <td>294</td>
      <td>2.84%</td>
    </tr>
    <tr>
      <th>58</th>
      <td>Road-150 Red, 48</td>
      <td>$640,510.33</td>
      <td>179</td>
      <td>179</td>
      <td>2.47%</td>
    </tr>
  </tbody>
</table>
</div>




```python

```
