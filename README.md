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
swan_first_pass.estimate_nonwear(df=dataframe object, sampling_rate=sampling rate of data)
```

To run swan second pass algorithm
```python
swan_second_pass.main(day_folder=path of the date folder)
```

You can also run 
```python
data = swan_first_pass.estimate_nonwear(df=dataframe object, sampling_rate=sampling rate of data)
result = swan_second_pass.correct_nonwear_predictions(data)
```

# Citation
Implementation mapped out in 
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9615811/
https://doi.org/10.1249%2FMSS.0000000000002973

> Thapa-Chhetry B, Arguello DJ, John D, Intille S. Detecting Sleep and Nonwear in 24-h Wrist Accelerometer Data from the National Health and Nutrition Examination Survey. Med Sci Sports Exerc. 2022 Nov 1;54(11):1936-1946. doi: 10.1249/MSS.0000000000002973. Epub 2022 Jun 23. PMID: 36007161; PMCID: PMC9615811.


