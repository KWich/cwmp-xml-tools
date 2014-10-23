# CWMP XML Tools

* see http://www.broadband-forum.org/cwmp for general information
* some additional documentation is available; refer to individual
  sub-directories

## Report_Tool: BBF Report Tool
* report.pl: perl script
* report.exe: standalone Windows executable (built using Strawberry Perl)
* report.darwin: standalone Mac OS X executable
* report.linux32: standalone Linux (32-bit) executable
* report.linux: standalone Linux (64-bit) executable
* plugins: example plugins, including:
  - plugins/instantiated: static instantiated data model tests
  - plugins/map: mapping from one data model to another

## ReportGUI: Graphical user interface for BBF Report Tool
* ReportGuiSetup.exe: Windows installer including report.exe and ReportGUI

## Publish_Tool: XML publication assistant (incomplete)
* publish.pl: perl script (processes XML and generates makefile)
* deps.pl: perl script (mini-make that can process the above makefile)

## MIB_Conversion_Tool: SNMP MIB to XML conversion
* mib2dm.pl: perl script (processes SMIv2 XML generated by smidump)

## XLS_Conversion_Tool: MSFT Excel table to XML conversion
* import.pl: perl script (processes Excel 2004 XML)

## DOC_Conversion_Tool: MSFT Word table to XML conversion (old)
* tr2dm.pl: perl script (processes DocBook XML generated by antiword)

## Threepio: XML parsing/tabling framework (old)
* src: source
	
## TRminator: XML parser/table tool (old)
* bin: binary jar file(s) for running TRminator "out of the box"
* doc: documentation directory
  - users_guide: guides to using the user interfaces of TRminator
  - dev_guide: guide to developing Threepio and TRminator
* src: source directory
  - threepio: source for the XML parsing/tabling framework
  - trminator: source for the BBF-specific processors and user interfaces that
    run on top of threepio
* T2: "JudgementDay" experimental build(s)
