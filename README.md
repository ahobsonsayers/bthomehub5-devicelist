# bthomehub5-devicelist
This library will return a dictionary containing information about the devices currently connected to a BT Home Hub 5 with a user specified IP Address.

## Installation

    pip install bthomhub5-devicelist

## How to use

Example Usage:

    import bthomehub5_devicelist
    from pprint import pprint
    
    
    def main():
        
        # If an IP Address is not specified, it will default as 192.169.1.254
        devicelist = bthomehub5_devicelist.get_devicelist('192.168.1.254')
    
        pprint(devicelist)
    
    
    if __name__ == '__main__':
        main()

The library will return a dictionary with connected devices MAC addresses as keys and device names as values

The console output from running the example code will look like this:

```
>>> 
{'4f:c9:32:04:d3:ec': 'Example-PC',
 '3f:6a:66:49:d4:16': 'Example-IPhone',
 '01:5d:e8:fb:c8:a9': 'Example-Smartlight',
 '65:10:5c:6d:d0:2b': 'Example-Android'}
```

## License

MIT - Feel free to go crazy with the code