<!-- default file list -->
*Files to look at*:

* [MainWindow.xaml](./CS/MainWindow.xaml) (VB: [MainWindow.xaml](./VB/MainWindow.xaml))
* [MainWindow.xaml.cs](./CS/MainWindow.xaml.cs) (VB: [MainWindow.xaml.vb](./VB/MainWindow.xaml.vb))
<!-- default file list end -->
# How to determine whether an indicator's value falls into a particular range


<p>In some cases, you need to know whether or not the current value of an indicator belongs to a particular range. This example shows how to create a state indicator that changes its color depending on the current range. </p>


<h3>Description</h3>

<p>In this example, the Circular gauge is created with three ranges and two empty sections. Initially the gauge&#39;s needle doesn&#39;t belong to any range, so the state indicator is painted as a gray ellipse.</p><p>To solve this task it&#39;s necessary to handle the <a href="http://documentation.devexpress.com/#WPF/DevExpressXpfGaugesRangeBase_IndicatorEntertopic"><u>IndicatorEnter</u></a> and <a href="http://documentation.devexpress.com/#WPF/DevExpressXpfGaugesRangeBase_IndicatorLeavetopic"><u>IndicatorLeave</u></a> events in the following way:<br />
- if a needle &#39;enters&#39; a range, it becomes painted with a range color;<br />
- if a needle &#39;leaves&#39; a range, it becomes painted in gray.</p><p>Note: In this example we set the <a href="http://documentation.devexpress.com/#WPF/DevExpressXpfGaugesValueIndicatorBase_IsInteractivetopic"><u>IsInteractive</u></a> property to<strong> True</strong>, so that you can click on a gauge and manually change the current needle value.</p>

<br/>


