
This is a generic Alert/popOver without transition delegates. PopOver base class has a header template whose card color , title and SubTitle text are changable.

```
# PopOverBaseViewController :
```

1. Returns closePressedCallback : must be implemented by subclass to dismiss popover
2. Stored Properties : subclass must override stored properties to get new title, subtitle, contentHeight
* viewContent should be added with contentsubview

```
# Example to add viewcontent :-
```

imageContentView.removeFromSuperview()
imageContentView.frame = viewContent.bounds
viewContent.addSubview(imageContentView)

In case of textInput override textfeild delegate methods to set offset of view if required: Please refer input viewcontroller for detailed implementation

Please see the popOverSampleUsage for details on calling and overriding popOverBaseClass

```
# Prerequisities :-
```
1. Utils.Swift
2. Custom font added to pList and Font folder should be imported
4. Add all assets from Assets.xcassets

-Important Informtion
 GenericPopOver is written for Portrait only and without using autolayouts so it is required to disable autolayout and size class in storyboard for subclasses.

