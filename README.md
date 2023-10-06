# WPF-Tab-Template
This sample code gives you an idea about how to use Tab ControlTemplate in WPF to create same layout for each tab that is created dynamically from code behind.
What's more, you can set the value of the textbox or get its value on any tabs.

As long as you use this command to set the tabControl's ItemsSource, whenever you add a new object of item to the 
TabCameraItems_Runtime, which is a "ObservableCollection", you can dynamically add a new tab to the TabControl.
This command can also be written after adding a new object of item to the TabCameraItems_Runtime.

```
 //各Tabが有する各Itemの値をUIに適用
TabControl1.ItemsSource = TabCameraItems_Runtime;

//Tabを１つ追加
TabCameraItems_Runtime.Add(new CameraItems_Runtime()
{
    ID = 11,
    FirstName = "Kapil",
    LastName = "Malhotra"
});

//Tabを１つ追加
TabCameraItems_Runtime.Add(new CameraItems_Runtime()
{
    ID = 22,
    FirstName = "Joe",
    LastName = "Yarbrough"
});
```
