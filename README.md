# SWaN_accel package

This is an algorithm to distinguish between sleep-wear, wake-wear, and non-wear in accelerometer dataset. 

To install the package, use the following pip command:
```python
pip install swan_accel
```

To import the two relevant methods from the package, type:
```python
from SWaN_accel import swan_first_pass, swan_second_pass
```
To run swan first pass algorithm:
```python
swan_first_pass.main(df=dataframe object, file_path=path for output file,sampling_rate=sampling rate of data)
```

To run swan second pass algorithm
```python
swan_second_pass.main(day_folder=path of the date folder)
```

You can also run 
```python
swan_first_pass.main(df=dataframe object, file_path=output_path,sampling_rate=sampling rate of data)
data = pd.read_csv(output_path)
result = swan_second_pass.correctPredictionsDataFrame(data)
```

