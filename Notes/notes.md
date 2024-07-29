##### debugShowCheckedModeBanner
- Hide the red tape
```
return MaterialApp(
      debugShowCheckedModeBanner: false,
      home: Scaffold()),
```
<img src="image.png"  width="200">
<img src="image-1.png"  width="200">

---
### ElevatedButton :
```
ElevatedButton(
  onPressed: () {},
  style: ElevatedButton.styleFrom(
    backgroundColor: Colors.orange[400],
    minimumSize: const Size(110, 40),
    shape: RoundedRectangleBorder(
      borderRadius: BorderRadius.circular(0),
    ),
  ),
  child: const Text(
    'Add 1 Point',
    style: TextStyle(
        color: Colors.black, fontWeight: FontWeight.w700),
  ),
)
```
![alt text](image-2.png)


---
### SizedBox :
- fixed size between widgets , better than ( Spacer ) widget
```
const SizedBox(
  height: 16
)
```
<img src="image-3.png"  width="100">


---
- Putting ( Row ) in ( Column ) and using ( Vertical Divider ), we must specifies the height of the divider
- using ( SizedBox )
```
const SizedBox(
  height: 400,
  child: VerticalDivider(
    thickness: 1,
    indent: 20,
  ),
)
```
<img src="image-4.png"  width="150">


---
### anonymous function :
- function used one time in their location
```
onPressed: () {}
```


---
### StatefulWidget :
- Used in case of widget with variable value
- It consists of the widget class (contain @override createState method) and the widget state
<img src="image-5.png"  width="400">


### setState
- Change the old state and show the new state (new changes)
```
setState(() {

});
```