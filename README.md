# AnchoredFloatView

***

This is a Float View to indicate the direction and quickly scroll up or down to the TableView selected Row.

It basically consists of a custom UILabel with one fixed UIImageView inside it, on the left.

![anchoredfloatview-preview](https://cloud.githubusercontent.com/assets/1878740/5674917/31940f0e-979a-11e4-94f3-f7c979dcc790.gif)

## Features

- automatically update label frame and align it on TableView bottom center 
- quickly scroll up or down the tableView to the selected row on click
- nice splash animation
- rotation compatible

## Installation

Grab the files in `View/AnchoredFloatView` and put it in your
project. The code uses ARC, so make sure to turn that on for the files if you're
not already using ARC.

## Usage

import the header class on your tableViewController:
```objectivec
#import "AnchoredFloatView.h"
```
alloc/init the view on viewDidLoad passing tableView and the indexPath of the selectedRow by parameter:
```objectivec
AnchoredFloatView *floatView = [[AnchoredFloatView alloc] initWithTableView:self.tableView andTargetIndexPath:self.targetIndexPath];
[self.view addSubview:floatView];
```

## Small Print

### License

`AnchoredFloatView` is released under the MIT license.

### Author

Carlos Arantes ([@carantes](http://twitter.com/carantes))
