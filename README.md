# Head First Python book - Notes

## Functions and Modules - Standard library
**1. sys module** 
- sys.platform
- print(sys.version) - Python version 
              
**2. os module**
- os.getcwd() - name of folder where the code is operating
- access system’s environment variables:
    * whole system
        ~~~python
        >>> os.environ 
        environ({'ALLUSERSPROFILE': 'C:\\ProgramData', 'APPDATA': 'C:\\Users\\lenka\\AppData\\Roaming', 
        'COMMONPROGRAMFILES': 'C:\\Program Files (x86)\\Common Files', 
        'COMMONPROGRAMFILES(X86)': 'C:\\Program Files (x86)\\Common Files', 
        'COMMONPROGRAMW6432': 'C:\\Program Files\\Common Files', 'COMPUTERNAME': 'ASUS-ZB-UX410UA', 
        'COMSPEC': 'C:\\WINDOWS\\system32\\cmd.exe', 'DRIVERDATA': 'C:\\Windows\\System32\\Drivers\\DriverData', 
        'FPS_BROWSER_APP_PROFILE_STRING': 'Internet Explorer', 'FPS_BROWSER_USER_PROFILE_STRING': 'Default'
        ~~~
    * individiual location
        ~~~python
        >>> os.getenv('APPDATA')
       'C:\\Users\\lenka\\AppData\\Roaming'
       ~~~          
       
**3. datetime module**
- date.today()
~~~python
>>> import datetime
>>> datetime.date.today()
datetime.date(2019, 5, 29)
~~~

- separetely
~~~python
>>> datetime.date.today().day
29
>>> datetime.date.today().month
5
>>> datetime.date.today().year
2019
~~~
