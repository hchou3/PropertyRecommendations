This is an app that generates comps for real estate properties. It uses euclidean distances between physical coordinates and property feature strings to calculate the most similar properties.

### Instructions:
  `pip install fuzzywuzzy geopy thefuzz`


## Step 1:
  load the JSON file
  `with open('appraisals_dataset.json', 'r') as f:
  data = json.load(f)
  df = pd.DataFrame(data)
  df = pd.json_normalize(df['appraisals'])`

## Step 2:
  Clean the features in dataframe in the section: Data Cleaning Pipeline
  Enter which row in the variable (i) for your training data

## Step 3:
   Format the data for Training in the Training secion
  
## Step 4:
  Use Euclidean Distances on the data points.
  Validate with RandomForestRegressor
