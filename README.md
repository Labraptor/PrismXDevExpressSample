# PrismXDevExpressSample Error
This project aims to illustrate the issue that arises in the TabViewItem when a value is assigned to the HeaderIcon property, when Prism and DevExpress are used together.

This problem only occur on iOS, no issue with Android

The TabViewItem.HeaderIcon is use in the MainPage.xaml

 <dxco:TabViewItem HeaderText="Mail" HeaderIcon="cloudsunaltsvgrepocom.png" HeaderVisibleElements="Icon" >
## Expected error
Exception has occurred: ObjCRuntime.ObjCException
Objective-C exception thrown.  Name: NSInvalidArgumentException Reason: *** -containsValueForKey: cannot be sent to an abstract object of class NSCoder: Create a concrete instance!
## Environment informations 
dotnet version : 8.0.204

| Installed Workload Id | Manifest Version | Installation Source |
|-----------------------|------------------|---------------------|
| maui-ios              | 8.0.7/8.0.100    | SDK 8.0.200         |
| maui-android          | 8.0.7/8.0.100    | SDK 8.0.200         |
| maui                  | 8.0.7/8.0.100    | SDK 8.0.200         |

## External dependecy used for this project : 

- "Prism.DryIoc.Maui" Version="9.0.179-pre" 
- "Prism.Maui" Version="9.0.179-pre" 
- "Prism.Maui.Rx" Version="9.0.179-pre" 
- "DevExpress.Maui.Controls" Version="23.2.5"
