## vba 문서 요약하기
### 2024.08.08 (https://learn.microsoft.com/en-us/office/vba/api/overview/excel)
#### 목차
1. 컨셉(Concpts)
2. 객체모델(Object Model)
3. 엑셀 그래프 비주얼 베이직 참조(Excel Graph Visual Basic reference)
##### 컨셉(Concepts)
###### 개요(Overview)
사용자에 의해 정의된 엑셀 솔루션을 개발하기 위한 중요한 컨셉들을 제공합니다. 왼쪽의 다양한 주제들을 패널을 통해 탐색할 수 있습니다. 
###### About the PowerPivot Model Object in Excel
~~~
Lean about the powerPivot add-in model and its object model in excel.
The powerpivot add-in enables you to visually build your own cubes.
A data cube is an array of data defined in dimensions or layers.
The Model object in Excel implemented by the Powerpivot add-in provides the foundation to load and combine source data from several data sources for data analysis on the destop, including relational databases,multidimensional sources, cloud services, data feeds, excel files, txt files, and data from the web.
Excel integrates additional data sources and enables the ability to combine data from multiple data sources.
~~~
~~~
> 파워 피봇의 add-in 모델과 객체 모델에 대해 알아보자
> 파워 피봇의 add-in은 큐브를 쌓는 것과 같다.
> 데이터가 들어간 큐브는 차원이나 레이어로 정의된 배열이다.
> 엑셀의 모델 객체는 파워 피봇의 add-in에 의해 구현된다. 
> 파워 피봇은 데이터를 로드하거나 소스 데이터를 결합하는 기반이 되고
> desktop에서 관계형 데이터 베이스, 다차원 소스, 클라우드 서비스, 데이터 피드 등과같은 데이터 분석 작업을 할 수 있게 해준다.
> 엑셀은 데이터를 통합하고 다양한 데이터 소스를 결합하는 능력을 가지고 있다.
~~~

~~~
The creation and deletion of the PowerPivot Model(PPM) is triggered by user exposed actions and cannot be created directly by the developer.
~~~

~~~
PPM의 생성과 삭제는 사용자가 사용할 수 있으며 개발자가 직접 사용하는 것이 아니다.
~~~

~~~
Relationships defined
Throughout this aticle, we will refer to the connection between two tables that establishes how the data should be correlated as relationships.

Relationships join together data from previously unrelated data sources. Each relationship has a primary Key and a forign key. Relationships allow the data to be joined together into a single model. This allows for:

Filtering data in one table by data in a related table
Filtering data by related columns
Integrating columns from multiple tables into a PivotTable/PivotChart
Keeping workbooks smaller by not having to repeat data
~~~

~~~
관계 정의
이 문서를 통해 두 테이블간의 연결이 되는지 알 수 있습니다.
서로 관계가 없던 데이터 간의 결합을 통해서 관계가 형성됩니다.
기본키와 외부키를 통해 이루어집니다.(row, column)
한 테이블과 관계된 다른 테이블로 필터링을 하거나 col를 기준으로 필터링 할 수도 있다.
피봇 테이블이나 차트를 이용하여 다시 데이터를 작성하지 않아도 원하는 col를 가지고 작업할 수 있어workbook을 작게 유지할 수 있다.   
~~~

~~~
Single Models Only
Excel with the PowerPivot add-in creates a single model in the workbook to which it can add data sources, create, modify, and relate tables. There can only be a single model in a workbook.
~~~

~~~
하나의 workbook에서 하나의 파워피봇만 생성하여 사용할 수 있다. 
~~~

~~~
Working with OLAP data sources
When connecting to an OLAP data source such as Analysis Services and creating OLAP PivotTables, PivotCharts, Slicers or Cube functions, no model is created. Workbooks created with the PowerPivot add-in can be uploaded to SharePoint, loaded in memory on the server, and accessed by other workbooks as if it were a normal instance of SQL Server Analysis Services.
~~~

~~~
OLAP data : Online Analytical Processing 데이터를 작업할 수 있다. 마이크로소프트가 만든 SharePoint 서비스가 있는데 이를 제공하는 서버의 메모리에 올려서 작업할 수 있다고 한다. 마찬가지로 마소에서 서비스하는 SQL Server Analysis Services에서도 사용할 수 있다.
~~~

~~~
Trigger the creation of a PowerPivot Model
By default, XLSX files in Excel 2010 and Excel don't have a PPM initialized in them until the model is deemed necessary. Certain actions trigger the creation of a PPM if there is no existing model in the workbook. The following sections describe the actions that will trigger the creation of a PPM when it does not exist in the workbook.
~~~

~~~

~~~


###### 함수(Functions)
###### 워크 북, 워크 시트(Wokbooks and worksheets)
###### 셀, 범위(Cells and rages)
###### 제어, 대화박스, 서식(Controls, dialog boxes, and forms)
###### 이벤트, 워크 시트 함수, 형태(Events, worksheet functions, and shapes)
###### 다른 프로그램에서 사용(Working with other applications)
###### 스파크라인(Sparklines)
###### 엑셀 성능(Excel performance)

##### 객체 모델(Object model)
###### 개요(Overview)

(https://tabletomarkdown.com/generate-markdown-table/)

| 번호 | 객체 이름 | 요약 |
| -- | ----- | -- |
|1|AboveAverage Object||
|2|Action Object||
|3|Actions Object||
|4|AddIn Object||
|5|AddIns Object||
|6|AddIns2 Object||
|7|Adjustments Object||
|8|AllowEditRange Object||
|9|AllowEditRanges Object||
|10|Application Object||
|11|Areas Object||
|12|Author Object||
|13|AutoCorrect Object||
|14|AutoFilter Object||
|15|AutoRecover Object||
|16|Axes Object||
|17|AxisTitle Object||
|18|Border Object||
|19|Borders Object||
|20|CalculatedFields Object||
|21|CalculatedItems Object||
|22|CalculatedMember Object||
|23|CalculatedMembers Object||
|24|CalloutFormat Object||
|25|CategoryCollection Object||
|26|CellFormat Object||
|27|Characters Object||
|28|Chart Object||
|29|ChartArea Object||
|30|ChartCategory Object||
|31|ChartGroup Object||
|32|ChartGroups Object||
|33|ChartObject Object||
|34|ChartObjects Object||
|35|Charts Object||
|36|ChartTitle Object||
|37|ChartView Object||
|38|ColorFormat Object||
|39|ColorScale Object||
|40|ColorScaleCriteria Object||
|41|ColorScaleCriterion Object||
|42|ColorStop Object||
|43|ColorStops Object||
|44|Comment Object||
|45|Comments Object||
|46|CommentThreaded Object||
|47|CommentsThreaded Object||
|48|ConditionValue Object||
|49|Connections Object||
|50|ConnectorFormat Object||
|51|ControlFormat Object||
|52|CubeField Object||
|53|CubeFields Object||
|54|CustomProperty Object||
|55|CustomProperties Object||
|56|CustomView Object||
|57|CustomViews Object||
|58|DataBar Object||
|58|DataBarBorder Object||
|59|DataFeedConnection Object||
|60|DataLabel Object||
|61|DataLabels Object||
|62|DataTable Object||
|63|DefaultWebOptions Object||
|64|Dialog Object||
|65|Dialogs Object||
|66|DialogSheetView Object||
|67|DisplayFormat Object||
|68|DisplayUnitLabel Object||
|69|DownBars Object||
|70|DropLines Object||
|71|Error Object||
|72|ErrorBars Object||
|73|ErrorCheckingOptions Object||
|74|Errors Object||
|75|FileExportConverter Object||
|76|FileExportConverters Object||
|77|FillFormat Object||
|78|Filter Object||
|79|Filters Object||
|80|Floor Object||
|81|Font Object||
|82|FormatColor Object||
|83|FormatCondition Object||
|84|FormatConditions Object||
|85|FreeFormBuilder Object||
|86|FullSeriesCollection Object||
|87|Graphic Object||
|88|Gridlines Object||
|89|GropShapes Object||
|90|HeaderFooter Object||
|91|HiLoLines Object||
|92|HPageBreak Object||
|93|HPageBreaks Object||
|94|Hyperlink Object||
|95|Hyperlinks Object||
|96|Icon Object||
|97|IconCriteria Object||
|98|IconCriterion Object||
|99|IconSet Object||
|99|IconSetCondition Object||
|100|IconSets Object||
|101|Interior Object||
|102|IRTDUpdateEvent Object||
|103|LeaderLines Object||
|104|Lengend Object||
|105|LengendEntries Object||
|106|LengendEntry Object||
|107|LengendKey Object||
|108|LinearGradient Object||
|109|LineFormat Object||
|110|LineColumn Object||
|111|LineColumns Object||
|112|ListDataFormat Object||
|113|ListObject Object||
|114|ListObjects Object||
|115|ListRow Object||
|116|ListRows Object||
|117|Mailer Object||
|118|Model Object||
|119|ModelChanges Object||
|120|ModelColumnChange Object||
|121|ModelColumnChanges Object||
|122|ModelColumnName Object||
|123|ModelColumnNames Object||
|124|ModelConnection Object||
|125|ModelFormatBoolean Object||
|126|ModelFormatCurrency Object||
|127|ModelFormatDate Object||
|128|ModelFormatDecimalNumber Object||
|129|ModelFormatGeneral Object||
|130|ModelFormatPercentageNumber Object||
|131|ModelFormatScientificNumber Object||
|132|ModelFormatWholeNumber Object||
|133|ModelMeasure Object||
|134|ModelMeasureName Object||
|135|ModelMeasureNames Object||
|136|ModelMeasures Object||
|137|ModelRelationship Object||
|138|ModelRelationships Object||
|139|ModelTable Object||
|140|ModelTableColumn Object||
|141|ModelTableColumns Object||
|142|ModelTableNameChange Object||
|143|ModelTableNameChanges Object||
|144|ModelTableNames Object||
|145|ModelTables Object||
|146|Model3DFormat Object||
|147|ModuleView Object||
|148|MultiThreadedCalculation Object||
|149|Name Object||
|150|Names Object||
|151|NegativeBarFormat Object||
|152|ODBCConnection Object||
|153|ODBCError Object||
|154|ODBCErrorS Object||
|155|OLEFormat Object||
|156|OLEObject Object||
|157|OLEObjects Object||
|158|Outline Object||
|159|Page Object||
|160|Pages Object||
|161|PageSetup Object||
|162|Pane Object||
|163|Panes Object||
|164|Parameter Object||
|165|Parameters Object||
|166|Phonetic Object||
|167|Phonetics Object||
|168|PictureFormat Object||
|169|PivotAxis Object||
|170|PivotCache Object||
|171|PivotCaches Object||
|172|PivotCell Object||
|173|PivotField Object||
|174|PivotFields Object||
|175|PivotFilter Object||
|176|PivotFilters Object||
|177|PivotFormula Object||
|178|PivotFormulas Object||
|179|PivotItem Object||
|180|PivotItemList Object||
|181|PivotItems Object||
|182|PivotLayout Object||
|183|PivotLine Object||
|184|PivotLineCells Object||
|185|PivotLines Object||
|186|PivotTable Object||
|187|PivotTableChangeList Object||
|188|PivotTables Object||
|189|PivotValueCell Object||
|190|PlotArea Object||
|191|Point Object||
|192|Points Object||
|193|ProtectedViewWindow Object||
|194|ProtectedViewWindows Object||
|195|Protection Object||
|196|PublishObject Object||
|197|PublishObjects Object||
|198|Queries Object||
|199|QueryTable Object||
|200|QueryTables Object||
|201|QuickAnalysis Object||
|202|Range Object||
|203|Ranges Object||
|204|RecentFile Object||
|205|RecentFiles Object||
|206|RectagularGradient Object||
|207|Research Object||
|208|RoutingSlip Object||
|209|RTD Object||
|210|Scenario Object||
|211|Scenarios Object||
|212|Series Object||
|212|SeriesCollection Object||
|213|SeriesLines Object||
|214|ServerViewableitems Object||
|215|ShadowFormat Object||
|216|Shape Object||
|217|ShapeNode Object||
|218|ShapeNodes Object||
|219|ShapeRange Object||
|220|Shapes Object||
|221|Sheets Object||
|222|SheetViews Object||
|223|Slicer Object||
|224|SlicerCache Object||
|225|SlicerCacheLevel Object||
|226|SlicerCacheLevels Object||
|227|SlicerCaches Object||
|227|SlicerItem Object||
|228|SlicerItems Object||
|229|SlicerPivotTables Object||
|230|Slicers Object||
|231|Sort Object||
|232|SortField Object||
|233|SortFields Object||
|234|SparkAxes Object||
|235|SparkColor Object||
|236|SparkHorizontalAxis Object||
|237|Sparkline Object||
|238|SparklineGroups Object||
|239|SparkPoints Object||
|240|SparkVerticalAxis Object||
|241|Speech Object||
|242|SpellingOptions Object||
|243|Style Object||
|244|Styles Object||
|245|Tab Object||
|246|TableObject Object||
|247|TableStyle Object||
|248|TableStyleElement Object||
|249|TableStyleElements Object||
|250|TableStyles Object||
|251|TextConnection Object||
|252|TextEffectFormat Object||
|253|TextFrame Object||
|254|TextFrame2 Object||
|255|ThreeDFormat Object||
|256|TickLabels Object||
|257|TimeLineState Object||
|258|TimeLineViewState Object||
|259|Top10 Object||
|260|TreeviewControl Object||
|261|Trendline Object||
|262|Trendlines Object||
|263|UniqueValues Object||
|264|UpBars Object||
|265|UsedObjects Object||
|266|UserAccess Object||
|267|UserAccessList Object||
|268|Validation Object||
|269|ValueChange Object||
|270|VPageBreak Object||
|271|VPageBreaks Object||
|272|Walls Object||
|273|Watch Object||
|274|Watches Object||
|275|WebOptions Object||
|276|Window Object||
|277|Windows Object||
|278|Workbook Object||
|279|WorkbookConnection Object||
|280|WorkbookQuery Object||
|281|Workbooks Object||
|282|Worksheet Object||
|283|WorksheetDataConnection Object||
|284|WorksheetFunction Object||
|285|Worksheets Object||
|286|WorksheetDataConnection Object||
|287|WorksheetFunction Object||
|288|Worksheets Object||
|289|WorksheetView Object||
|290|XmlDataBinding Object||
|291|XmlDataMap Object||
|292|XmlDataMaps Object||
|293|XmlNamespace Object||
|294|XmlNamespaces Object||
|295|XmlSchema Object||
|295|XmlSchemas Object||
|296|XPath Object||



