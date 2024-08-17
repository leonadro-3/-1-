## vba 문서 요약하기

## 처음 공부시 크게 중요하지 않은 챕터
---------------------------------------
### 2024.08.08 (https://learn.microsoft.com/en-us/office/vba/api/overview/excel)
#### 목차
1. 컨셉(Concpts)
2. 객체모델(Object Model)
3. 엑셀 그래프 비주얼 베이직 참조(Excel Graph Visual Basic reference)
##### 컨셉(Concepts)
###### 개요(Overview)
사용자에 의해 정의된 엑셀 솔루션을 개발하기 위한 중요한 컨셉들을 제공합니다. 왼쪽의 다양한 주제들을 패널을 통해 탐색할 수 있습니다. 
###### 1.About the PowerPivot Model Object in Excel 
###### 2.About coauthoring
###### 3.Language-specific properties, methods, and functions 
###### 4.OLE DB for OLAP properties used by Excel 
###### 5.Programming for the single document interface in excel
> 1~5 의 내용은 수많은 object 들에 대한 정의나 추상적인 정의를 나열하고 있다. 영어로 엑셀 문서에 무료로 자원봉사를 하고 싶다면 굳이 말리진 않겠다.
---------------------------------------
---------------------------------------
##### 함수(Functions)
###### Using the Solver VBA Functions(VBA 함수들을 이용하여 실재로 사용하는 예제들)
엑셀에 solver 기능이 있는데 solver 사용시 실행되는 함수들이라고 생각하면 된다. 이런식으로 어떤 함수가 GUI 제공되어 직관적으로 알 수 있다.   
예를들어 pyautogui의 경우 이러한 gui 기반의 기능을 조합하여 사용하는 것이라고 생각하면 된다.   

###### SolverAdd Function
###### SolverChange Function
###### SolverDelete Function
###### SolverFinish Function
###### SolverFinishDialog Function
###### SolverGet Function
###### SolverLoad Function
###### SolverOk Function
###### SolverOkDialog Function
###### SolverOptions Function
###### SolverReset Function
###### SolverSave Function
###### SolverSolve Function
---------------------------------------
---------------------------------------
###### 워크 북, 워크 시트(Wokbooks and worksheets)
###### 셀, 범위(Cells and rages)
###### 제어, 대화박스, 서식(Controls, dialog boxes, and forms)
###### 이벤트, 워크 시트 함수, 형태(Events, worksheet functions, and shapes)
###### 다른 프로그램에서 사용(Working with other applications)
###### 스파크라인(Sparklines)
###### 엑셀 성능(Excel performance)

##### 객체 모델(Object model)
## 처음 공부시 크게 중요하지 않은 챕터
---------------------------------------
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

---------------------------------------

