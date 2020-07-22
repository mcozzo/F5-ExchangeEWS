# F5 iRule for Exachange access to EWS

## Steps
1. Create iRule and import code
2. Create iRule Data Group List
    1. Local Traffic > iRules > Data Group List
    2. Create a new list named *Exchange_EWS_Allowed_IP* Type = Address
    3. Add addresses to the list using the following convention: [Address] := [Value]
    ```
    10.0.0.0/8 := RFC1918-10
    172.16.0.0/12 := RFC1918-172
    192.168.0.0/16 := RFC1918-192
    ```
