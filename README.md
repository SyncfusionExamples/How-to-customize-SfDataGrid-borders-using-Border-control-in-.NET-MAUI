# How to customize SfDataGrid borders using Border control in .NET MAUI?
This demo shows how to customize SfDataGrid borders using Border control in [.NET MAUI DataGrid](https://help.syncfusion.com/maui/datagrid/overview)(SfDataGrid). 

By default, the .NET MAUI SfDataGrid displays only horizontal grid lines. If you want to show an outer border around the entire DataGrid, you can wrap the SfDataGrid inside a Border control. This allows you to visually enhance the grid by adding a clear boundary around it.

## Xaml
```
 <ContentPage.BindingContext>
     <local:OrderInfoRepository x:Name="viewModel" />
 </ContentPage.BindingContext>

 <Border WidthRequest="600">
     <Grid>
     <syncfusion:SfDataGrid x:Name="dataGrid" VerticalOptions="CenterAndExpand"
                            ItemsSource="{Binding OrderInfoCollection}">
         <syncfusion:SfDataGrid.Columns>
             <syncfusion:DataGridNumericColumn HeaderText="Order ID" Format="0"
                                             MappingName="OrderID" Width="150"/>
             <syncfusion:DataGridTextColumn  HeaderText="Customer"
                                             MappingName="Customer"
                                             Width="150" />
             <syncfusion:DataGridTextColumn  HeaderText="Ship City"
                                             MappingName="ShipCity"
                                             Width="150" />
             <syncfusion:DataGridTextColumn  HeaderText="Ship Country"
                                             MappingName="ShipCountry"
                                             Width="150" />
         </syncfusion:SfDataGrid.Columns>
     </syncfusion:SfDataGrid>
     </Grid>
 </Border>

```

## Requirements to run the demo

To run the demo, refer to [System Requirements for .NET MAUI](https://help.syncfusion.com/maui/system-requirements)

## Troubleshooting:
### Path too long exception

If you are facing path too long exception when building this example project, close Visual Studio and rename the repository to short and build the project.

## License

Syncfusion has no liability for any damage or consequence that may arise from using or viewing the samples. The samples are for demonstrative purposes. If you choose to use or access the samples, you agree to not hold Syncfusion liable, in any form, for any damage related to use, for accessing, or viewing the samples. By accessing, viewing, or seeing the samples, you acknowledge and agree Syncfusion's samples will not allow you seek injunctive relief in any form for any claim related to the sample. If you do not agree to this, do not view, access, utilize, or otherwise do anything with Syncfusion's samples.