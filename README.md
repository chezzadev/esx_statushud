# esx_statushud


### Images


### Requirements
![alt text](https://i.gyazo.com/86847c95fc4219926c9d4b342c2f3349.png "Logo Title Text 1")

### Installation 
* Drag **esx-statushud** folder into your resources and add to your **server.cfg** under the required scripts.
* Open **esx_status/client/main.lua** and replace line `71` with the `New Line` below.

Original Line:
```lua
TriggerEvent('esx_status:onTick', GetStatusData(true))
```
New Line:
```lua
TriggerEvent('esx_statushud:onTick', GetStatusData(true))
```
* Open **esx_basicneeds/client/main.lua** and change values of lines `43` and `49` to `false`.

Original Line:
```lua
return true
```
New Line:
```lua
return false
```