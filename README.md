# DialogBoxForMaterialDesignInXamlToolkit
This is the repo to host the source code for MaterialDesign DialogBox that behaves like MessageBox in WinForms. So just use it like you do when you use MessageBox!

## Prerequisite
You have to [install](https://github.com/ButchersBoy/MaterialDesignInXamlToolkit/wiki/Super-Quick-Start) MaterialDesignInXamlToolkit before you use this library. 

## How to use ?
### To show one button only : 
```C#
DialogBox.Show("ERROR 404", "Unable to connect to the website.", "RETRY");
```
![image](https://user-images.githubusercontent.com/23183656/30526968-c2c5ade4-9c55-11e7-969a-2c5a90c6e1ba.png)


### To show two buttons : 
```C#
DialogBox.Show("ERROR 404", "Unable to connect to the website. Do you want to retry?", "ABORT", "RETRY");
```

![image](https://user-images.githubusercontent.com/23183656/30526979-fc8f2a8c-9c55-11e7-9fe2-882599eab1c2.png)
### To know user clicked which button : 
```C#
switch (DialogBox.Result) {
    case DialogBox.Result_.LeftButtonClicked:
        MessageBox.Show("You clicked left button");
        break;
    case DialogBox.Result_.RightButtonClicked:
        MessageBox.Show("you clicked right button");
        break;
}
```
