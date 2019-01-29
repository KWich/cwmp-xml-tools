ReportGUI:
==========

This utility provides a graphical front-end for the "report.exe" tool from BroadnamdForum to generate reports from CWMP
and USP XML data model files.

The Windows installer includes the front-end and the actual report.exe tool. For installation please 
execute the ReportGuiSetup and follow the instructions. The tool runs under Windows (7, 8, 10)

For questions and comments please use the build in feedback function.


History
--------
2019/01/31 ReportGuiSetup 4.0, ReportGui 4.0, report.exe#422+ (report.pl#422) 
    new version of report.exe (report.pl#422+) included in installer
    new ReportGui version 4.0
    - Support for USP and CWMP data models
    - Button "Show Report" now automatically checks for existing reports and warns if these are missing or outdated.
    - New option to automatically generate XML catalog file from include directories. 
      (e.g. to cover development versions of cwmp-datamodel-1-x.xsd)
    - Reworked update functions to cope with new BBF web page structure 
    Note 

2017/09/07 ReportGuiSetup 3.3, ReportGui 3.3, report.exe#421 (report.pl#421)
    new version of report.exe (report.pl#421) included in installer
    new ReportGui version 3.3
    - Drag n Drop of XML Files into Selection file
    - Generated files are now in central output directory (Setting - "Select output directory") 
    
2017/06/14 ReportGuiSetup 3.2, ReportGui 3.2, report.exe#420 (report.pl#420)
    new version of report.exe (report.pl#420) included in installer
    new ReportGui version 3.2
    - fix wrong link in upgrade procedure
    
2017/01/31 ReportGuiSetup 3.0, ReportGui 3.1, report.exe#404 (report.pl#404)
    new ReportGui version 3.1
    - uses BBF GITHUB repository instead of UNH repository for update checks

2017/01/31 ReportGuiSetup 3.0, ReportGui 3.0, report.exe#404 (report.pl#404)
    new version of report.exe (report.pl#404) included in installer
    new ReportGui version 3.0
    - adapted to work with new BBF web-page layout
    - Log limit increased
    - Unused options "use old XML" removed

2013/09/11 ReportGuiSetup 2.6, ReportGui 2.6, report.exe#277 (report.pl#277)
    new version of report.exe (report.pl#277) included in installer
    new ReportGui version 2.6
    - XML download adapted to new BBF web page
    - publish options adapted to new format
    - publishing without warnings report as default 

2013/11/11 ReportGuiSetup 2.5, ReportGui 2.5, report.exe#251 (report.pl#251)
    new version of report.exe (report.pl#251) included in installer
    new ReportGui version 2.5
    - installer fixes

2012/11/25 ReportGuiSetup 2.4, ReportGui 2.4, report.exe#209 (report.pl#209)
  new ReportGui version 2.4:
  - Changed functions:
    * Sort report setting default is now "False"
    * Setting "set report tool" now allows also to select the Perl script directly
    * Icons and colors adapted
  - New functions:
    * New Option Extras->"Create CWMP Index page" to create index pages according to OD-290 
      during publishing (report.hmlbbf)
      The creation can also be included in the publishing automatically with the settings 
      Extras->"Include CWMP Index page in publish all files"
      
2012/04/13 ReportGuiSetup 2.3, ReportGui 2.3, report.exe#209 (report.pl#209)
  new version of report.exe (report.pl#209) included in installer
  new ReportGui version 2.3:
  - New functions:
    * New setting to sort reports. If enabled all reports will be generated with the 
      --sortobjects option available with report.exe#209. Option defaults to "True"
    * Support for plug-ins in the Expert mode. Plug-ins can in the <programdir>\plugins directory 
      be selected via drop down list to be executed during report generation
  
2012/02/29 ReportGuiSetup 2.2, ReportGui 2.2, report.exe#206 (report.pl#206)
  new ReportGui version 2.2:
  - Changed functions:
    * HTML report functions now generates generic HTML with the --nomodels --automodel 
      option for component models
    * Publish uses option -loglevel=w1 for all reports
    * Publish additional generates generic HTML with the --nomodels --automodel option 
      for component models
    * Publish log includes program version
    * new formatted output, differentiated by error, warning, indent
    * Select new report tool: confirmation in log file
    * improved windows resize to adapt to screen, keep item positions, minimum size 500x580
  - New functions:
    * log level can be selected in panel, output split depending on log level
    * New option: Check for new file from BBF home page
  - Fixed Error(s):
    * Capital spelling for options Showdiffs and Lastonly removed

2011/12/09 ReportGuiSetup 2.1, ReportGui 2.1, report.exe#198 (report.pl#198)
  new version of report.exe (report.pl#198) included in installer
  bug fixes and enhancements:
  * perform report tool updates with administrative rights
  * compact command output for readability, new option to show command string
  * input field for additional include directories extended 
  * Publish all does not work from any directory due to missing include of own directory
  * time stamps for generation
  * new naming conventions for generated XMLs: last becomes diffs and all becomes full
  * new Setting "Use Old XML names" to switch back to old naming conventions
  * automatic adaptation of window height to vertical screen size

2011/08/15 ReportGuiSetup 2.0, ReportGui 2.0, report.exe#186 (report.pl#186)
  new version of report.exe (report.pl#186) included in installer
  new ReportGui version 2.0:
  - Changed functions:
    * ReportGui now runs with user rights under Windows 7, INI file was moved into %USER/appdata 
      directory
    * Deprecated 'noautomodel' option replaced with new option 'automodel'
    * 'ShowDiffs' option added to expert mode and as option to standard html reports
    * Report.exe output separated for errors and statistics
    * New setting to show or hide statistic display
    * Publish option also generates flattened XML file
  
  - New functions:
    * New option to download all released XML and schema files from BBF website into default
      include directory
    * New upgrade option to check for new versions
    * "Publish all files" option to generate files to be published for a whole directory
    * New feedback option
    
  - Fixed Error(s): 
    * Error checking crashed program, due to variable error

2011/02/24 ReportGuiSetup 1.0.6, ReportGui 1.1, report.exe (report.pl#182)
  new version of report.exe (report.pl#182) included in installer.

2011/02/11 ReportGuiSetup 1.0.5, ReportGui 1.1, report.exe (report.pl#181) 
  Update ReportGUI 1.1 :
  - New standard report options to compare two files
  - Improved handling of include directories, possible to sort list. 
  - prevent overwrite of source XML for XML targets in expert handling

2011/01/25 ReportGuiSetup 1.0.4, ReportGui 1.0.2
  new version of report.exe (report.pl#181) included in installer. 
  Error correction in ReportGUI: Include directories and filenames with spaces are now correctly processed

2010/11/20 ReportGuiSetup 1.0.3, ReportGui 1.0.1
  new version of report.exe (report.pl#177) included in installer. 
  
2010/10/14 ReportGuiSetup 1.0.2, ReportGui 1.0.1
  new version of report.exe (report.pl#175) included in installer. 
  Installer will now override report.exe during reinstall if it includes newer version.

2010/10/08 ReportGuiSetup 1.0.1, ReportGui 1.0.1 
  new version of report.exe (report.pl#174) included in installer. 
  Please uninstall old version first.