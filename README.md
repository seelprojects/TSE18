# TSE18
TSE18 is a tool to visualize the performance of 4 Information Retrieval (IR) methods: Vector-Space Model (VSM), Latent Semantic Indexing (LSI), Jensen-Shannon Model (JSM), and Pointwise Mutual Information (PMI) on bug localization.

![ScreenShot](https://github.com/seelprojects/TSE18/blob/master/src/image.jpg)

### Getting Started
TSE18 is a single file .exe tool that can be run without any external support. The main window provides following options:

#### Dataset
User can choose one of more dataset to visualize. Dataset available are for AspectJ, Eclipse, JodaTime, SWT, and ZXing.

#### Method i
User can choose one or more IR methods. These methods will be treated and base method to which another method will be combined.

#### Method j
User can choose one or more IR methods. Each of these method will be combined to each of the methods in Method i.

#### Metric
User can choose one metric. The performance will be evaluated based on the metric. Available metrics are Top Rank (TR) 1, Top Rank 5, Top Rank 10, Mean Average Precision, and Mean Reciprocal Rank.

#### Setting
This section provided settings to edit the graphs generated. 
- X-Min: the minimum value in x-axis
- X-Interval: the interval used for x-axis
- X-Max: the maximum value in x-axis

- Y-Min: the minimum value in y-axis
- Y-Interval: the interval used for y-axis
- Y-Max: the maximum value in y-axis

- Width: the width of each graph
- Height: the height of each graph

### Development Environment
In order to open and modify the C# source project you will need:
- Visual Studio 2015 [Free Community Edition](https://www.visualstudio.com/en-us/products/visual-studio-community-vs.aspx)
- [.Net 4.5.2](https://support.microsoft.com/en-us/kb/2901907)

Once available, open BugLocalizationHybridApproach.sln in [src](src/) directory in Visual Studio.

### Resources
The performance metric for all projects and method combinations are provided as an XML format. Users can find the XMLs in [src/BugLocalizationHybridApproach/Resources](src/BugLocalizationHybridApproach/Resources/).