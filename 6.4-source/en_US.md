> This article was translated by machine.

# Changelog Version 6.4

## 6.4.16

### CAD
#### "Recent Projects" Menu

In CAD, there is a submenu "Recently edited projects" in the "Project" menu. In the CAD Options dialog (System->Project) the user can define which project information is displayed in the submenu. After a new installation, the headings were displayed in the "Projects last edited" menu. If you switched to the opton dialog, the field "Designation" was incorrectly selected there. 

After an installation, the default for displaying the most recently edited projects is the generic term.

Translated with www.DeepL.com/Translator

#### Print project

In CAD, you can use the "Print project" function to print several files of a project one after the other. After calling this function, the "Page Setup" dialog appears. If the print preview was selected here, the print output was started immediately.

The error has been corrected.

### CAD Schaltplan-Assistent

#### Save labeling settings as default

Some labeling settings are saved in Treesoft CAD in the file apar.dat. This file is copied from the AppData directory of the system to the new project directory when a new project is created. Since the settings stored in the file apar.dat in the AppData directory could not be changed until now, the labeling parameters usually had to be adjusted after creating a new project.

In the Options dialog, it is now possible to overwrite the basic settings of the label paranters stored in the apar.dat file. For this there is a new button Standard in the toolbar of the dialog. The following settings are saved:

- Labelling rule
- Labeling mode
- Bmks always new assigned
- Suggest potentials and terminals
- Upper limit for path texts
- Lower limit for path texts

#### Comments on "Save As"

In Treesoft CAD, files can be assigned comments that describe the content of the respective file. With the "Save as" function there was no possibility to enter a comment text. 

The dialog "Save as" has been extended by an input field "Comment". If the file to be saved has already been assigned a comment, this is displayed. The input field is combined with a selection list from which predefined comments can be selected from the standard file for comment texts. Only comments on drawings (files with the extension .zng) are displayed in the selection list.

#### Open file, save file as

In CAD, there have been various dialogs for opening drawing files. In the Options dialog Schematic->File one could choose one of three possible variants, which should be used when opening files[Ctrl]+[O].

In the future, the document window will be displayed when opening drawings[Ctrl]+[O]. In addition, it is possible to use the file dialog with the[F8] key. In the same way, press the[F9] key to call up the "Save as" function.

#### Single/Mark All

In the Schematic Editor, the texts to be labeled can be individually defined in the "Label individually" or "Label all" dialogs. It was not possible to restore the delivery state.

There is now a "Delivery status" button in the toolbar. This function restores the settings.

#### Bmk Selection

In the dialogs for BmK selection for terminals, potentials, contacts, PLCs and cables, the "Matchcode" input field always had the focus after opening, recognizable by the blinking cursor. To enter a new device designation, you first had to switch to the next input field "BmK" using the[Tab] key, for example.

After opening the dialogs for the BmK selection, one of the two input fields "Matchcode" and "BmK" now always gets the focus, which last had the focus the last time it was opened. This property is managed separately for each resource type.

#### Number range for dummies

When creating new dummies, it was previously not possible to select a number using an appropriate number range.

The function is now available. The number is determined by clicking with the left mouse button on the text "Number:", which is displayed as a hyperlink.

#### Save symbol as, select catalog branch

When creating symbols only the symbol library in which the symbol is to be saved and a corresponding comment could be entered. An assignment to a catalog branch was not possible.

When saving symbols, you can now directly select a branch of your own catalog.

#### Change article assignment

In Treesoft CAD, articles can be assigned to symbols relevant for evaluation. To do this, you will find the two options "Assign articles individually" and "Assign all articles" in the "Symbol" menu. The "Change article assignment" menu option determines whether only symbols that have not yet been assigned an article or all symbols are to be taken into account. Therefore, if you wanted to change the article of a certain symbol, you had to activate this option first.

The menu option "Change article assignment" only applies to the command "Close all articles". In the "Assign article individually" function, however, the symbol closest to the crosshair position is always processed, regardless of whether an article has already been assigned to it or not.

#### Repeat function "W"

If you set a symbol as a graphic in the "Set article/symbol" function and then moved the crosshairs with the keyboard to another position, the repeat function ([W] key) did not work. The function could only be called when the mouse button was pressed.

This error has been corrected.

#### File new

Comments on files can be stored in Treesoft CAD. For most drawing files the comments are predefined and stored in the file describe.dat in the AppData directory. When creating a new drawing in the Schematic Editor, a comment could be entered, but a suitable predefined comment was not suggested.

When creating a new drawing file, a default comment is now preset.

#### Content n Label

In the "Text" menu, there was the menu option "Frame&variable "Label content n"...". 

Since this function can only be used to label the two variables "Contents 1" and "Contents 2", the command has been renamed "Label Contents 1/Contents 2".

#### Assigning Articles from External Catalog

When you assign articles to symbols, all articles for which the respective symbol is primarily or secondarily assigned are offered for selection. If an article from a foreign catalog is added to the selection list, the assignment of the article to the relevant symbol is saved in the database as a secondary reference. If no symbol is assigned to the newly assigned article, no direct assignment has been made in the copy of the article in the Own Catalog.

If new articles are selected when symbols are labelled to which no symbol has yet been assigned, a primary assignment is automatically created.

#### Create/change free text

A context menu is displayed in the Schematic Editor when the right mouse button is pressed. Before the menu is displayed, the system first checks which objects are near the crosshair position. If the next object is a text, the additional option "Create / edit free text" is offered in the context menu. However, the search for a text was only carried out if there were free texts on the visible layers; symbol texts were not taken into account. This made it difficult, for example, to label the drawing frame in an otherwise empty file.

The search for a text is now always performed if there are free texts or symbol texts on the visible layers.

#### Automatic BmKs for terminals and cables

In Treesoft CAD, the user can choose between different algorithms for the marking of equipment, according to which the equipment is to be marked. Previously, when labelling terminals and cables, the user could only enter the BmK manually or select an already assigned device designation from a list. As a rule, the device identifiers of terminals and cables are assigned according to the labeling rule "Bmk/lfd". With extensive circuit diagrams, it could be cumbersome to determine the next BmK not yet assigned. Some users, in turn, use the "sheet/path" algorithm when labeling terminals or cables. Previously, these BmKs had to be entered manually.

To meet the above requirements, the dialogs for entering and selecting device identifiers for terminals and cables have been extended. There is now a button directly next to the "BmK:" input field. A new BmK is generated according to the labeling rule "Bmk/lfd" and transferred to the input field "BmK". The focus also changes to the input field, so that the dialog can be ended directly with the enter key. The next time the labeling dialog for an unlabeled terminal or cable is called, the previously automatically generated BmK is preselected in the list (as with manual input), since the labeling rule "Bmk/lfd" is mainly used for the resolved display of devices.
Another new "Suggest Bmk" control allows the user to specify whether a suggestion is to be displayed in the selection list according to the set labeling rule. This suggestion is always at the top of the list and can be accepted immediately after opening the respective dialog for unlabeled terminals or cables with the enter key. The next time the labeling dialog for an unlabeled terminal or cable is called, the first entry in the list is preselected again, since this form of labeling is used for devices that are not displayed in expanded form. As a result, a new bmk is usually requested.

#### Blanks in plant and location identifier

If system or location designations with spaces were used in the schematic, the abbreviated notation of the device designations did not work.

The error has been corrected.

#### Set article/symbol

In the Set article symbol function, articles or symbols are selected from a list for each catalog. If you started the evaluation with the list open, you could no longer navigate with the arrow keys in the list.

The error has been corrected.

#### Variablentext

Unlike other texts, variable texts have additional specifications that are called variable types. The type of variable is set in a separate dialog when creating texts. The next new variable text to be created should be assigned the last selected variable type. However, the variable type was not restored correctly.

The error has been corrected.

#### Assign article

In the Set article/symbol function, material, services and dummies were displayed alternately in separate lists. A common list of different master data could not be displayed.

The "Assign article" dialog has been completely revised so that all master data to which the symbol to be labeled is assigned is now displayed together in a list. In addition, some changes have been made to the handling of the dialog in order to meet the new requirements and to make operation simpler and more transparent.

#### Set article/symbol

If an article was selected in the "Set article/symbol" function to which the 0artvari macro was assigned, the crosshair was not on the reference point of the symbol after the assigned symbol was positioned.

The error has been corrected.

#### Unnecessary menus and options

The Schematic Wizard menus contained some unnecessary commands that were removed. The Options dialog has also been cleaned up.

Cleansing the menus.

#### Set raster graphics

When inserting a raster graphic into a drawing, it is possible to position or scale it. This is done via the "Raster Graphics" dialog, in which further parameters can be set. However, the content of the dialog was updated with every mouse movement, so that a reasonable parameterization of the raster graphics was not possible.

The error has been corrected.

#### SPS-Assignment definition

Using the "Define PLC assignment list" function, text module files for CAD are generated from sequential assignment lists or vice versa. The first time you call it up in a project, the directory of the assignment list was not preset. Furthermore, the directory of the project was preset for the text module file and not the respective subdirectory TreeCAD.

When the function is called for the first time in a project, both directories are preset to the CAD subdirectory of the active project. The settings of the dialog are then saved in the file "ZolTbs.def" in the respective project.

#### Project path is not saved when registering a project

Before projects can be edited in Treesoft CAD, they must be saved in the database. Among other things, the function "Register project" is used for this purpose. In some cases, after registering a project, the directory path of the project was not saved and therefore no access to the files was possible. The reason for this was that the project was already stored in the database and had a delete or archive mark. For example, projects that are logged off are not removed from the database, but are only marked for deletion. Deleted or archived projects are not visible in CAD and cannot be edited. When attempting to submit such a project, the problem described above occurred.

When registering a project, the system now checks whether a suitable data record already exists in the database that has been marked for deletion or archiving. In this case, an error message appears.

#### Automatic wire numbering

In CAD, it is possible to have vein symbols set automatically between two interconnected devices. There are numerous setting options for wire numbering, including the user can determine the type of numbering and the numbering sequence. In the combination of the numbering type "Sheet/Pathwise" and the numbering sequence "left-right/top-down", the first wire number to be assigned was always started when changing the path, even if wire numbers were already assigned in the path above the wire symbol to be labeled.

The error has been corrected.

#### BmK frame in the evaluation

In CAD, you can use BmK frames to assign parts of a sheet to another system or location indicator. During the evaluation, the level assignment of the BmK frames was not correctly considered in all cases, so that incorrect cross-references were generated.

The error has been corrected.

#### Set article/symbol

In the Set article/symbol function, material, services and dummies were displayed alternately in separate lists. A common list of different master data could not be displayed. 

The dialog has been completely revised so that all master data are now displayed together in a list. In addition, some changes have been made to the handling of the dialog in order to meet the new requirements and to make operation simpler and more transparent.

#### Macro 3spsbgtd.mac

With the macro 3spsbgtd.mac PLC assemblies with partial representations are defined. The dialog could neither be closed with the Enter key nor with the[ESC] key. The "Copy" and "Paste" buttons also did not work. In the dialog "Label symbol texts automatically" only one element of the list could be brought into edit mode by double-clicking the left mouse button. The list element in the background flickered. Also this dialog could not be closed with the[Enter] or[Esc] key.

The "Copy" and "Paste" functions in the "PLC component parameters" dialog box have been removed, as they can only be displayed on the current database structure with considerable effort. Alternatively, you can first create a copy of the article and then parameterize it. Please note that when changing the symbol assignments for a copied article, the function "Assign symbol texts automatically" must always be called up for the overall display and for each partial display. This is the only way to ensure that only those texts are labeled that use this as a placeholder in the symbols.
The "Automatically label symbol texts" dialog now essentially consists of a combination of an input field and a list. The possible symbol texts for labeling are displayed in the list and the text to be labelled of the selected symbol text can be entered in the input field. With the arrow keys "up" and "down" as well as with the mouse wheel you can navigate in the list without losing focus. In this way, the texts to be labeled can be entered very quickly.

### CAD Stammdaten

#### Parameter cable/conductor

To define a cable/cable, the macro 0cables is assigned to the species data in CAD. When the "Circuit diagram parameters" button is pressed, the "Cable/line parameters" dialog box appears, in which specific data for a cable or a line are stored. When creating new cores, the number of cores must first be defined, which are then displayed in the "Define cores individually" list field. If you changed the focus to this list field, its content was deleted.

The error has been corrected.

### CAD Konverter

#### Maximum number of objects exceeded

If the maximum number of objects was exceeded during the export to ZNG, the user was not notified. Despite the message "Export successful" the exported drawing did not contain all objects.

The user is now informed that the maximum number of objects is exceeded. It is possible to cancel the process and subsequently select another drawing as the destination for the export. To simplify this process, the functionality of the "Reassign" command has been extended.

#### Buttons remain disabled after a command is executed

It could happen that some buttons were not reactivated after executing a command.

The respective buttons are now correctly reactivated.

#### Expansion of export area not recalculated

It could happen that the expansions of export areas were not recalculated when objects were moved or deleted in the drawing.

The expansions of the export areas are now recalculated after changes to the drawing.

#### Drawing incorrectly conveyed

It could happen that the drawings to be exported were misplaced if an export area was changed in batch export mode for the control technology.

The drawings to be exported are now transferred correctly.

### Adressverwaltung

#### Adding customer/employee or supplier/manufacturer information

In the Treesoft Office start center, the addresses last edited are also displayed. When adding customer/employee/supplier or manufacturer information to an address, this address was not added to the list of recently edited addresses.

When adding customer/employee/supplier or manufacturer information, this address is now also added to the list of recently edited addresses. This means that you can now also access these addresses very quickly via the Start Center.

#### Create contact person, first name is recognized incorrectly

When a contact person is created, the software automatically recognizes the title, title, first name and surname and automatically fills in the letter salutation. With the name "Frauke", or "Herrmann", the first name was cut off, as it is also part of the salutation.

This misbehaviour has been corrected. The letter salutation is now also filled in for first names, the part of the salutation are correct.

### Mailing

#### Attachments

When sending an e-mail with attachments, it could happen that the attachments were sent and saved as mailatt*. This could only happen if the e-mail was opened from the drafts, then printed and sent directly afterwards.

The e-mails are now also sent and saved in the above constellation with the correct names for file attachments.

#### Optimization of speed in multiple sending

Before a multiple transmission, a filter is executed that restricts the data records and selects the communication. In multiple transmission, the address information for variable replacement was read out again for each individual address with the complete conditions of the filter. For more complex filters, this meant that several seconds could elapse between processing each e-mail.

When reading the address information for variable replacement, the address is only selected after the address ID from the already executed filter. This is much faster and leads - regardless of the complexity of the filter - to a constant time per address.

### Stammdaten

#### Parameter macro 0ArtVari

The parameter macro 0artvari is used to automatically label certain symbol texts after setting an article. When selecting the text formats, it was not possible to select auxiliary variables, device designators and comment texts. In certain situations, the input field was also preassigned with a blank character.
The "Copy" and "Paste" functions, which can be called via buttons in the toolbar, are used to conveniently label several symbols with identical symbol texts. The "Copy" function creates a list with the symbol texts and the texts to be entered. For each text found in the list, the "Insert" function preassigns the respective contents of the list to the "Label with" column. You should be able to edit the list created with the "Copy" function in the set editor using the "Text storage" function. However, the list was searched in an incorrect directory. 

Access to the list of copied texts works again. The dialog "Edit multiline texts" is now called modally, i.e. it must be closed before a new text can be selected from the list for editing.
When selecting the text formats, auxiliary variables, device designators and comment texts can now also be selected specifically. The input field is no longer preassigned with a blank character. 
The symbol texts found are displayed sorted by text format in the following order:

- Information variables
- Supplementary variables
- auxiliary variables
- Equipment identification
- Connection texts
- mirror texts
- Comment texts

#### Select services, dummies, parameter macro

Parameter macros differ from other macros by special functions. The first time a parameter macro is selected (or using the "Refresh" function in the "Select parameter macro" dialog), a list of all available parameter macros is created. For this purpose, all macros of the system are loaded once and checked accordingly. Here several messages appeared in succession that certain macros could not be read.

The error has been corrected.

#### Dialog Choose Parametermacro

At a low resolution the dialog box Select parameter macro was opened too small. The minimum height of these dialogs was one fifth (20%) of the available height of the screen.

The minimum height of these dialogs is now one fourth (25%) of the available screen height.

#### Button Circuit diagram parameters/switch cabinet parameters

Articles, parameters for the schematic or control cabinet assistant can be stored. A parameter macro can be selected for this purpose. The parameters entered are then saved in the respective data record of the article, i.e. the article must already exist in the database. When creating new articles, both buttons were deactivated, i.e. an article had to be created first. Only then could the parameters be entered via an assigned macro.

To simplify the creation of new articles, parameters can now already be assigned when entering the article data. The user is asked to save the data set so that the parameters to be entered have a home address.

#### Schematic Parameters button

Dummies can be used to store parameters for the Schematic Editor. A parameter macro can be selected for this purpose. The parameters entered are then saved in the respective data record of the dummy, i.e. the dummy must already exist in the database. When creating new dummies the button was deactivated, i.e. a dummy had to be created first. Only then could the parameters be entered via an assigned macro.

To simplify the creation of dummies, you can now assign parameters when entering the dummy data. The user is asked to save the data set.

#### Create Dummys

In Treesoft CAD, dummies serve as placeholders for cross-reference-relevant components. The system uses the number and type of contacts actually assigned in the schematic to determine the contact mirror to be used during the evaluation by determining the optimum contact combination from the contact combinations stored in the dummy and inserting the assigned article into the schematic. The order in which the contact combinations are stored in the dummy plays a decisive role. For this reason it is possible to sort the contact combination. If this function was called when a dummy was created, all other input fields were deleted.

The error has been corrected.

#### Material, Service and Dummy

In the master data dialogs there were the buttons "Select macro". When this button was pressed, all macros of the system were offered for selection. However, only certain macros, so-called parameter macros, can be assigned to the master data. These are selected via the "Circuit diagram parameters" or "Control cabinet parameters" button. 

The above buttons have been removed.

### Offene Posten Verwaltung

#### Selecting a painting in the dunning run

We have newly developed the selection dialogs for mailings, filters and texts and integrated them into Treesoft Office. Since this integration, it was no longer possible to select or change a mailing when executing a dunning run using the"..." button. The change or selection of a mailing could only be made in the Options dialog > Basics > Dunning > Dunning run.

You can now also select a direct mailing in the dunning run window.

### ERP Dokumente

#### Program aborts during preview/printing and booking

When calling the preview/print and posting a document, the program was usually terminated with an error message.

We have removed the last changes from the ERP and will analyze the program termination in more detail. This means that the preview/printing and posting of ERP documents functions again as before.

### Installation

#### Synchronization hangs if a file without file extension is found

Synchronization of the local network installation could hang if a file with an empty file extension was retrieved via a UNC path.

The synchronization now also recognizes files without file extension and is executed as expected.

### System

#### Global keyboard shortcuts

In the TreesoftOffice there are some global key combinations that allow a quick change between different windows/functions of the software. Only a few of them were implemented in CAD. Here, it was only possible to call up the functions via the "Window" menu.

Below is a list of the global key combinations implemented in CAD:

- [Shift]+[Ctrl]+[F3] = Startcenter
- [Shift]+[Ctrl]+[P] = Projects
- [Shift]+[Ctrl]+[A] = Addresses
- [Shift]+[Ctrl]+[H] = History
- [Shift]+[Ctrl]+[D] = Events
- [Shift]+[Ctrl]+[T] = Todos
- [Shift]+[Ctrl]+[C] = Calendar
- [Shift]+[Ctrl]+[E] = Dossier
- [Shift]+[Ctrl]+[L] = Window-List

#### Windows 10 detection

Microsoft will make the Windows 10 operating system available from 29.07.2015.

As long as we have not yet officially released Treesoft Office for Windows 10, a message will appear at program start.

### Mobile Anbindung

#### Search in daily planner

In the daily planner there is a search function to filter the displayed data, as in all other lists of the app as well. However, the search was not performed here, which is why there was no visible change to the list.

It is now possible to search in the day planner as usual.

#### Confirmation via result sets in the search functions

The search functions did not give a decent response about the result set if no match was found.

A message with "No data" is now displayed in the middle of the list as soon as no results are delivered for the search pattern.

#### full-text search

A search query was sent each time the key was pressed, if typing was too fast the user was brought to the login screen if necessary.

The full text search is now only executed after 0.5 seconds after the typing has stopped, as you are used to in TreesoftOffice.

#### Reloading addresses in the full text search

In the full-text search it was fixed that only the first 25 results are displayed from the search result.

It is now possible in the full text search to reload the results of the search and thus not only to display the first 25 results.

### Treesoft Backup Manager

#### Validation of the database backup

Previously, the database was backed up via Firebird during the database backup with Treesoft Backup Manager. There was no validation of the created backup.

As of version 6.4, the database backup is directly validated when a database backup is created. This ensures that the backup created has already been tested once and is functioning in the event of a restore.

### Plug-in Manager

#### Check if a plug-in is compatible

Until now it was possible to install a plug-in in every Treesoft Office 6.x version independently of the Treesoft Office version in which a plug-in was created. This is one of the biggest advantages but also a very big potential for errors. With version 6.4, not a single plug-in created in an earlier version can be imported, since the Firebird server takes the encoding very precisely and all older plug-ins have confused things here.

The Treesoft Plug-in Manager now checks if the plug-in is compatible with the version. If you try to import a plug-in that was created with a previous version in version 6.4, the import is prevented.

## 6.4.15

### CAD Konverter

#### Creation of export area not possible

It could happen that the creation of an export area in the model space layout with the message "No export areas can be created in a paper space layout". was denied.

The Model Space layout is now recognized as such.

### Adressverwaltung

#### Transfer Tax Code and Terms of Payment from Customer Master

On the Customer Information tab in an address, a user can specify that the tax code and terms of payment are selected by default when an ERP document is created. Previously, you could also activate the radio button if no tax code or payment term was selected. In some cases, this led to an unexpected program termination when creating an ERP document.

When you activate these radio buttons for tax codes and terms of payment, we now make sure that a tax code or a payment term has been selected beforehand.

#### Display the subject of the appointment or task in the resubmissions

The start on, main group and group of the task or appointment were displayed in the address resubmissions. For a better overview of addresses with several tasks or appointments, the subject of the respective task or appointment was missing.

For a better overview, the "Subject" column of the task or appointment is now also displayed in the address resubmission. Since this new column requires the delivered column sort to be adjusted, the column sort of the address list is reset to its default state with this update. However, the user can redefine the column sequence after the update if required.

#### Duplicate entries

From the lists in the address management it is possible to duplicate an entry to the current one, another one or to a project. This entry is missing in the main menu for the entries in the address management. Here it is only possible to duplicate a history entry, but not appointments and tasks.

The main menu in the address management for the entries has been extended. It is now possible to duplicate entries in the same way as from the lists.

### ERP

#### Program abort when calling up the document or position settings

In Treesoft Office you can set default settings for payment terms and tax codes in the customer information for an address. If you selected the options "Transfer payment terms from customer" or "Transfer tax code from customer" when creating a document and none were stored in the customer information of the address, then the program terminated unexpectedly when you added items and called up the settings from a position and the document.

When selecting the options, the system now checks whether the information is stored at the respective address. If not, the user has the option to switch to the address and change it or not to use this option.

### Einträge

#### Updating the calendar after a change in an appointment or task

The calendar has not automatically updated itself if a task or an appointment has been processed from another program position.

The calendar now updates itself automatically when saving tasks and appointments and displays the tasks and appointments correctly.

### ERP-Schnittstelle

#### Support of the Sage New Classic 2016

The Sage New Classic 2016 (version 5.3.4) was made available via live update.

Treesoft Office now supports the ERP interface version 2016.

## 6.4.14

### Mailing

#### Names of attachments in emails

When sending e-mails via the e-mail editor, you can select files from the hard disk and assign them as attachments to the e-mail. Until now it could happen that the file name in the sent e-mail was different from the one displayed in the e-mail editor. But the content of the file was always correct.

We now make sure that the names displayed in the e-mail editor for attachments are actually used when sending them.

### Stammdaten

#### Structure time of the material list

Since the database server was converted to Firebird 2.5, customers with material catalogs of approx. 400,000 data records have experienced a noticeable extension of the list development time.

The structure of the list was accelerated by optimizing the SQL statement, and is now measurably faster than with Firebird 2.1.

### Start-Center

#### Widget settings are lost

The column settings of the widgets in the Start Center could be lost and were reset to a default.

The column settings of the widgets in the Start Center are now saved and restored correctly.

## 6.4.13

### CAD Konverter

#### Crash during export to ZNG

Infinite lines (Xlines) could cause the software to crash when exporting DWG/DXF drawings to ZNG.

Xlines are now taken into account during export and no longer cause the software to crash.

### Notifier

#### Date display of tasks and appointments

The name of the date in the notification of tasks and appointments caused confusion in some cases. It was not directly apparent whether the date refers to the creation date or the Begins On date of the task.

The identifiers for tasks and appointments have been revised. Further information has also been added to the ToolTips.

#### Linked addresses for tasks are not displayed

If addresses outside the Notifier change, the display in the Notifier may not be updated correctly.

The Notifier now tries to monitor all known information for it and display all changes live. Due to time-critical circumstances, in individual cases it can still lead to a changed address still being displayed with the old name. After a one-time update, the information is always up-to-date and no restart of the notifier is required to resolve this circumstance.

### Einträge

#### E-mail inbox and e-mail outbox

In some cases it could cause the list of e-mails to be empty, but a record was displayed in the preview window.

The list of emails and the preview window are now synchronous and do not display incorrect records.

### ERP

#### Transfer of proposed invoice amounts

If an invoice was created with cash discount and the proposed incoming payment was to be transferred without cash discount, although cash discount deduction was possible, the cash discount was still always deducted.

Now the values clicked on during the transfer are correctly copied from the proposed line.

### Mobile Anbindung

#### HTTP connection

An iOS update has changed the default policies for connections to servers. By default, HTTP connections are now blocked and only HTTPS is allowed.

It is now possible to establish a connection via the HTTP protocol again.

## 6.4.12

### CAD Schaltplan-Assistent

#### Assigning articles with the parameter macro 0artvari

The parameter macro 0artvari is used to automatically label certain symbol texts after selecting an article. If the function "Assign article individually" was selected from the menu and an article to which the 0artvari macro is assigned was selected from the selection list displayed afterwards, no symbol texts were labeled.

The error has been corrected.

### CAD Konverter

#### Error when importing ZNG drawing

The import of ZNG drawings was aborted with an error message if the drawing contained texts with negative height.

Texts with a negative height no longer cause the import to terminate. In addition, it is now possible to set whether texts with a negative height are to be exported.

### Einträge

#### Rights for entries

With the rights management of Treesoft Office you can limit the visibility of entries. If you created the history entry via the edit pen in the Treesoft Notifier or the call dialog in the address management, then no rights were set for the entry, so that this entry was visible to everyone.

When logging calls via the call dialog or the Treesoft Notifier, the rights are now set according to the following rule. The default rights of the addresses are added together with the phone number, and if the current user is in one of the rights explicitly or in a group, the cumulative default rights are set, otherwise the entry is public and visible to everyone.

### Mailing

#### Inbox rights

With the rights management of Treesoft Office you can limit the visibility of entries. In some circumstances, the rights for the emails were not set as expected and defined so that these entries were visible to everyone.

When an e-mail is received, the rights are now set according to the following rule. If there are default rights for the addresses with the sender e-mail address, then these and the users named in AN and CC are added together and assigned to the e-mail. If there are no default rights for the addresses, the e-mail remains public. Only if no address is found in CRM, then the default right of the e-mail account is read out and if it is not public then additively composed with the users in AN and CC of the e-mail and assigned to the e-mail, otherwise the e-mail is public.

## 6.4.11

### CAD Konverter

#### Only one export range of a drawing is exported

Only one export area of a drawing was exported, no matter how many export areas were created.

All created export areas are exported again.

#### Incorrect export/import of multiline texts

Up to now, the position of multiline texts was not adjusted during both import and export. As a result, it could happen that line feeds up, alignment left/right down or rotations change the display of texts after conversion.

After converting from and to DWG/DXF, multi-line texts should now look like the original.

#### Open drawing gezoomed on extension

If a ZNG file converted to DWG/DXF format was opened in a third-party CAD program, the drawing extension had to be zoomed in to view the drawing.

During the conversion, corresponding parameters are now set so that the drawing converted into DWG/DXF format can be directly viewed in third-party programs.

#### Window position is saved

So far, no positions of the windows and dialogs have been saved.

Both the main window and the export dialog now save and restore the positions.

#### More memory can be addressed

Up to now, the CAD converter could only address up to 2 GiB of the available main memory, even in a 64 bit operating system.

The CAD converter can now address up to 4 GiB of the available main memory in a 64 bit operating system.

#### Incorrect positioning for bidirectional import

The positioning of the objects could differ on the Y-axis if the configuration file was created with version 6.4.8 or earlier or if the exported floor plan was moved.

In both cases, the objects are now positioned correctly.

### Start-Center

#### Menu blocks CAD/CRM/ERP via setting in the Show/Hide Options dialog box

The main menus CAD, CRM and ERP were always displayed in the start center.

Every user now has the possibility to show and hide the individual menus and program parts. For this purpose, a tab has been added to the Start Center branch of the Options dialog in the Basics area to configure the menu blocks.

### Notifier

#### Opening a project

The Notifier does not allow you to call up a project from a displayed task or appointment.

It is now possible to call up the linked projects from a displayed task or appointment using the context menu. It is also possible to assign a new project to a task or an appointment.

### Einträge

#### Display of abbreviations in the IDs column

In the list of entries, the IDs column displays the abbreviations of the assigned contact persons. If two contact persons had the same abbreviation, it was only displayed once, although several contact persons are linked to the entry.

All abbreviations of the assigned contact persons are now displayed, even if they duplicate each other. This makes it easier to see in the list whether one or more contact persons are linked.

## 6.4.10

### Projektverwaltung

#### End of program when changing the settings of a project

If the software was inactive or if the settings of a project were processed for a longer period of time, it could automatically end with the error message "invalid BLOB id.

The project list as well as the settings of a project are now kept up-to-date, so a longer editing of the settings can no longer lead to the state "invalid BLOB id.

### Mobile Anbindung

#### Stability of full text search improved

With heavily frequented or parallel queries to the full text search, it could happen that the Mobile Agent refused full text search queries.

The Mobile Agent is now prepared to process highly frequented and parallel full-text search queries.

### CAD Plug-in

#### New Treesoft CAD symbol catalogue QIVICON

QIVICON is an initiative of Deutsche Telekom AG with leading German industrial companies. QIVICON enables the cross-manufacturer and cross-brand networking of a smart home.

With the new Treesoft CAD symbol catalogue Qivicon we provide you with the articles and symbols of home automation of the manufacturer consortium QIVICON for project planning in building technology.

## 6.4.9

### Notifier

#### Display of addresses for calls

Which information of the found address is displayed in the Notifier can be set in the Options dialog > Basics > Computer Telephony, default is Name1 and Contact person. For calls - regardless of whether incoming or outgoing - from phone numbers the personal addresses are stored, "There is no address linked to this entry" was displayed although the phone number was stored at an address.

With this update, the name of the address is displayed again in this constellation.

### Mobile Anbindung

#### Deleted addresses are displayed

Deleted or archived addresses were displayed in the full text search and in the addresses.

Deleted or archived addresses are no longer displayed in the full text search.

#### Incorrect display in the communications/information on a contact person

When selecting a contact person, another contact person displayed the data for that contact person.

The correct information about the contact person is now displayed.

#### Using the full text search

When using the full text search by a mobile device, too many search results could result in the Mobile Agent not responding to any further requests from a client.

The bug that caused this was fixed. The full text search now also works for many results in the Mobile Agent.

### CAD Plug-in

#### New Treesoft CAD symbol catalogue Loxone Smart Home

In the Loxone Smart Home, a central device - the intelligent Loxone Miniserver - controls everything. From shading to music to heating.

With the new Treesoft CAD symbol catalogue Loxone Smart Home we make the articles and symbols of Loxone Smart Home available to you for project planning in the PLC Assistant.

#### New Treesoft CAD Symbol Catalog WAGO-I/O-System

Modular WAGO-I/O-SYSTEM, IP20 (Series 750/753). The WAGO-I/O-SYSTEM, with its fine-modular and fieldbus-independent design, meets the requirements of decentralized fieldbus systems in particular.

With the new Treesoft CAD symbol catalogue WAGO-I/O-System we provide you with the articles and symbols for planning the modular WAGO-I/O-Syxstem, IP20 (series 750/753).

## 6.4.8

### System

#### Support for Windows Server 2003 and Server 2003 R2 discontinued

On July 14, 2015 Microsoft discontinued extended support for Windows Server 2003 and Windows Server 2003 R2.

With the end of Microsoft support, we also end support for the server operating system.

## 6.4.7

### CAD Konverter

#### Open CAD converter after adding multiple files

When adding DWG/DXF files to a project, the CAD converter was opened with these files. If the files to be opened were in a path with spaces, then the CAD converter was started, but the added files were not opened.

After adding DWG/DXF files to a project, the CAD converter is also started for files whose path contains spaces and the transferred files are opened directly.

### Projektliste

#### Sort by creator or user

With Treesoft Office 6.4, sorting by creator or user in the project list resulted in no results being displayed. Instead, only the "Please wait a moment..." was displayed.

It is now possible to sort the project list by creator or user.

### System

#### Calling the "Text format" function

If the "Text format" function was started and ended in the "Foreign language translation" function, this dialog was repeatedly displayed when the cross-hairs were moved.

The error has been corrected.

## 6.4.6

### Stammdaten

#### Services: parameter macro

If a parameter macro was assigned to a newly created service, this was not saved.

The error has been corrected.

## 6.4.3

### CAD Schaltplan-Assistent

#### Maximum number of cores for cable definitions

Previously, only cables with a maximum of 120 cores could be defined.

The maximum number of cores per cable definition has been increased to 500.

## 6.4.2

### System

#### Treesoft Office und Taskleiste in Windows anheften

For a faster start of programs in Windows, frequently used programs are often pinned to the taskbar. However, this was not possible on a workstation of a Treesoft Office client server installation; the context menu only displayed the item "Close window". However, if Treesoft Office was installed on a single workstation, Treesoft Office could be attached to the task bar.

From this version it is now also possible to pin Treesoft Office to the task bar on a workstation in client server operation.
