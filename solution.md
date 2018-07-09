
# Create an Address on Testnet

#### Create a testnet address using your own secret key
#### (use your phone number if you can't think of anything)
#### Record this secret key!


```python
from ecc import G

# use your phone number if you can't think of anything
secret = 1800555555518005555555

# get the public point
point = secret*G
# if you completed the `address` method, just do the .address(testnet=True) method on the public point
print(point.address(testnet=True))
```
