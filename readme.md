#Loop viewpager helper
无限滚动的viewpager，当itemCount>1时，通过左右各增加一页，并在status是idle时定位到正确位置    
例如3个item
```text
       ┏━┓ ┏━┓ ┏━┓     
       ┃0 ┃ ┃1 ┃ ┃2 ┃     
       ┗━┛ ┗━┛ ┗━┛        
┏━┓ ┏━┓ ┏━┓ ┏━┓ ┏━┓    
┃2 ┃ ┃0 ┃ ┃1 ┃ ┃2 ┃ ┃0 ┃     
┗━┛ ┗━┛ ┗━┛ ┗━┛ ┗━┛
  0      1     2      3      4  
``` 

当滚动到4位置时，idle后定位到0，同理到0时idle定位到4，其他位置-1    
