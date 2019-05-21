# Python Docstrings

## Content

* `example_google.py`: This module demonstrates documentation as specified by the `Google Python Style Guide`.
  Source: https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html 

## Example for function

```python
def price_num(price_str):
    """Re-encode string of a dollar amount to float.
    
    Args: 
        price_str (str): Price value with dollar symbol and comma 
    
    Returns: 
        np.float32
        
    """
    if isinstance(price_str, str):
        return np.float32(price_str[1:].replace(',', ''))
    else:
        return np.nan
```
