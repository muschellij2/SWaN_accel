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
swan_first_pass.first_pass_nonwear(df=dataframe object, sampling_rate=sampling rate of data)
```

To run swan second pass algorithm
```python
swan_second_pass.main(day_folder=path of the date folder)
```

You can also run 
```python
data = swan_first_pass.first_pass_nonwear(df=dataframe object, sampling_rate=sampling rate of data)
result = swan_second_pass.correct_nonwear_predictions(data)
```

