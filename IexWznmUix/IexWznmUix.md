User interface ``[IexWznmUix]``
===

Schema
---

![](./IexWznmUix.jpg)

<p align="center"><em>Figure 1: User interface schema - table columns in light blue are part of the input file, table columns in dark blue are inferred</em></p>

Structure
---

[//]: # (IP structure - BEGIN)

<br>&nbsp;&nbsp;&nbsp;&nbsp;\+ Card [``[ImeIMCard]``](#1-card-imeimcard)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Control [``[ImeIMControl1]``](#11-control-imeimcontrol1)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Parameters [``[ImeIAMControlPar1]``](#111-parameters-imeiamcontrolpar1)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Name by locale [``[ImeIJMControlTitle1]``](#112-name-by-locale-imeijmcontroltitle1)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Dialog [``[ImeIMDialog]``](#12-dialog-imeimdialog)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- TblWznmCControl [``[ImeICControl3]``](#121-tblwznmccontrol-imeiccontrol3)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Control [``[ImeIMControl3]``](#122-control-imeimcontrol3)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Parameters [``[ImeIAMControlPar3]``](#1221-parameters-imeiamcontrolpar3)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Stub by vector item [``[ImeIJMControl3]``](#1222-stub-by-vector-item-imeijmcontrol3)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Name by locale [``[ImeIJMControlTitle3]``](#1223-name-by-locale-imeijmcontroltitle3)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Feed [``[ImeIMFeed3]``](#1224-feed-imeimfeed3)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Vector [``[ImeIMVector3]``](#12241-vector-imeimvector3)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Panel [``[ImeIMPanel]``](#13-panel-imeimpanel)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- TblWznmCControl [``[ImeICControl2]``](#131-tblwznmccontrol-imeiccontrol2)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Control [``[ImeIMControl2]``](#132-control-imeimcontrol2)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Parameters [``[ImeIAMControlPar2]``](#1321-parameters-imeiamcontrolpar2)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Stub by vector item [``[ImeIJMControl2]``](#1322-stub-by-vector-item-imeijmcontrol2)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Name by locale [``[ImeIJMControlTitle2]``](#1323-name-by-locale-imeijmcontroltitle2)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Feed [``[ImeIMFeed2]``](#1324-feed-imeimfeed2)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Vector [``[ImeIMVector2]``](#13241-vector-imeimvector2)
<br>&nbsp;&nbsp;&nbsp;&nbsp;\+ Presetting [``[ImeIMPreset]``](#2-preset-imeimpreset)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Name by locale [``[ImeIJMPresetTitle]``](#21-name-by-locale-imeijmpresettitle)
<br>&nbsp;&nbsp;&nbsp;&nbsp;\+ Query [``[ImeIMQuery]``](#3-query-imeimquery)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Clauses [``[ImeIAMQueryClause]``](#31-clauses-imeiamqueryclause)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Order rules [``[ImeIAMQueryOrder]``](#32-order-rules-imeiamqueryorder)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Query column [``[ImeIMQuerycol]``](#33-query-column-imeimquerycol)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Stub by presetting [``[ImeIJMQuerycolStub]``](#331-stub-by-presetting-imeijmquerycolstub)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Query modifier [``[ImeIMQuerymod]``](#34-query-modifier-imeimquerymod)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ TblWznmRMQueryMTable [``[ImeIRMQueryMTable]``](#35-tblwznmrmquerymtable-imeirmquerymtable)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- TblWznmTMQuerymodMQuery [``[ImeITMQuerymodMQuery]``](#351-tblwznmtmquerymodmquery-imeitmquerymodmquery)
<br>&nbsp;&nbsp;&nbsp;&nbsp;\- TblWznmRMPanelMQuery [``[ImeIRMPanelMQuery]``](#4-tblwznmrmpanelmquery-imeirmpanelmquery)

[//]: # (IP structure - END)

Details
---

### 1 Card ``[ImeIMCard]``

[//]: # (IP ImeIMCard.superUse - BEGIN)

Use:

[//]: # (IP ImeIMCard.superUse - END)

[//]: # (IP ImeIMCard.columns - BEGIN)

Column|Content|
-|-|
sref (string)|identifier|

[//]: # (IP ImeIMCard.columns - END)

### 1.1 Control ``[ImeIMControl1]``

[//]: # (IP ImeIMControl1.superUse - BEGIN)

Super import: card (1:N)

Use:

[//]: # (IP ImeIMControl1.superUse - END)

[//]: # (IP ImeIMControl1.columns - BEGIN)

Column|Content|
-|-|
srefIxVBasetype (string)|type<br>alr: alert<br>but: button<br>chk: checkbox<br>cpt: caption<br>csi: color signal<br>cus: custom<br>dit: dialog item<br>dld: file download link<br>dse: dialog item selector<br>hdg: heading<br>hsb: horizontal scroll bar<br>lsb: list scroll bar<br>lst: list<br>mcb: multiple-choice button<br>men: menu<br>mit: menu item<br>msp: menu separator<br>mrl: URL menu item<br>mtx: menu item text display<br>pup: pop-up menu<br>rbu: radio button<br>sep: separator<br>sge: stage information<br>sld: slider<br>spc: spacer<br>tbl: table<br>tco: table column<br>tos: table order selector<br>trs: table row selector<br>tsb: table scroll bar<br>txf: text field<br>txt: text display<br>upd: up/down<br>uld: file upload field<br>vsb: vertical scroll bar|
srefHkIxVSection (string)|hook<br>void: none<br>mbar: menu bar<br>side: side<br>hdr: header<br>hdrdetd: header when detached<br>hdrregd: header when regularized<br>cont: content<br>contdetd: content when detached<br>contregd: content when regularized<br>tbl: table<br>ftr: footer|
srefRefIxVTbl (string)|reference<br>void: none<br>dlg: dialog<br>qco: query column<br>rel: relation<br>tbl: table<br>tco: table column|
srefRefUref (string)|reference|
srefSupRefWznmMControl (string)|super control|
supNum (uint)|super control|
srefIxVScope (string)|scope<br>app: app only<br>shr: shared app/engine|
sref (string)|identifier|
srefIxVSubtype (string)|subtype<br>void: none<br>ditstd: custom single<br>ditarr: custom arrayed<br>ditdld: download<br>dituld: upload<br>ditprg: progress|
srefsWznmMTag (string)|tag|
Avail (string)|availability rule|
Active (string)|activation rule|
srefsKOption (string)|options<br>bicol: bi-column<br>cap: capitalized title<br>ddd: title complement ' ...'<br>flexh: flexible height<br>icon: icon<br>iframe: inline frame<br>live: live data display<br>log: logarithmic scale<br>multsel: multiple item selection<br>mdnup: mouse down/up tracking<br>onoff: on and off states<br>rast: value raster<br>s: small<br>t: tall<br>tmstamp: time stamp scale<br>tmdate: date scale<br>tmtime: time scale<br>tricol: tri-column<br>xs: extra small|

[//]: # (IP ImeIMControl1.columns - END)

### 1.1.1 Parameters ``[ImeIAMControlPar1]``

[//]: # (IP ImeIAMControlPar1.superUse - BEGIN)

Super import: control (1:N)

Use:

[//]: # (IP ImeIAMControlPar1.superUse - END)

[//]: # (IP ImeIAMControlPar1.columns - BEGIN)

Column|Content|
-|-|
x1SrefKKey (string)|key<br>action: triggered action<br>cptwidth: caption width<br>height: height<br>icon: icon<br>stdicon: standard icon<br>width: width|
srefX2RefWznmMLocale (string)|locale|
osrefKVal (string)|value<br>crdopen: open card<br>dlgopen: open dialog<br>dlgclose: close dialog|

[//]: # (IP ImeIAMControlPar1.columns - END)

### 1.1.2 Name by locale ``[ImeIJMControlTitle1]``

[//]: # (IP ImeIJMControlTitle1.superUse - BEGIN)

Super import: control (1:N)

Use:

[//]: # (IP ImeIJMControlTitle1.superUse - END)

[//]: # (IP ImeIJMControlTitle1.columns - BEGIN)

Column|Content|
-|-|
srefX1RefWznmMLocale (string)|locale|
Title (string)|Title|

[//]: # (IP ImeIJMControlTitle1.columns - END)

### 1.2 Dialog ``[ImeIMDialog]``

[//]: # (IP ImeIMDialog.superUse - BEGIN)

Super import: card (1:N)

Use:

[//]: # (IP ImeIMDialog.superUse - END)

[//]: # (IP ImeIMDialog.columns - BEGIN)

Column|Content|
-|-|
srefIxVBasetype (string)|type<br>new: new record<br>select: record select<br>filter: list filter configuration<br>mnrel: m:n relation<br>mnnew: m:n attribute  new<br>import: data import<br>export: data export<br>jump: jump table edit<br>rights: user rights<br>report: report generation<br>cust: custom|
srefRefIxVTbl (string)|reference<br>void: none<br>tbl: table<br>rel: relation<br>iex: import/export complex|
srefRefUref (string)|reference|
sref (string)|identifier|
Comment (string)|comment|

[//]: # (IP ImeIMDialog.columns - END)

### 1.2.1 TblWznmCControl ``[ImeICControl3]``

[//]: # (IP ImeICControl3.superUse - BEGIN)

Super import: dialog (1:N)

Use:

[//]: # (IP ImeICControl3.superUse - END)

[//]: # (IP ImeICControl3.columns - BEGIN)

Column|Content|
-|-|
iref (ubigint)|ref|

[//]: # (IP ImeICControl3.columns - END)

### 1.2.2 Control ``[ImeIMControl3]``

[//]: # (IP ImeIMControl3.superUse - BEGIN)

Super import: dialog (1:N)

Use:

[//]: # (IP ImeIMControl3.superUse - END)

[//]: # (IP ImeIMControl3.columns - BEGIN)

Column|Content|
-|-|
iref (ubigint)|ref|
srefIxVBasetype (string)|type<br>alr: alert<br>but: button<br>chk: checkbox<br>cpt: caption<br>csi: color signal<br>cus: custom<br>dit: dialog item<br>dld: file download link<br>dse: dialog item selector<br>hdg: heading<br>hsb: horizontal scroll bar<br>lsb: list scroll bar<br>lst: list<br>mcb: multiple-choice button<br>men: menu<br>mit: menu item<br>msp: menu separator<br>mrl: URL menu item<br>mtx: menu item text display<br>pup: pop-up menu<br>rbu: radio button<br>sep: separator<br>sge: stage information<br>sld: slider<br>spc: spacer<br>tbl: table<br>tco: table column<br>tos: table order selector<br>trs: table row selector<br>tsb: table scroll bar<br>txf: text field<br>txt: text display<br>upd: up/down<br>uld: file upload field<br>vsb: vertical scroll bar|
irefRefWznmCControl (ubigint)|TblWznmCControl|
srefHkIxVSection (string)|hook<br>void: none<br>mbar: menu bar<br>side: side<br>hdr: header<br>hdrdetd: header when detached<br>hdrregd: header when regularized<br>cont: content<br>contdetd: content when detached<br>contregd: content when regularized<br>tbl: table<br>ftr: footer|
srefRefIxVTbl (string)|reference<br>void: none<br>dlg: dialog<br>qco: query column<br>rel: relation<br>tbl: table<br>tco: table column|
srefRefUref (string)|reference|
irefSupRefWznmMControl (ubigint)|super control|
srefIxVScope (string)|scope<br>app: app only<br>shr: shared app/engine|
sref (string)|identifier|
srefIxVSubtype (string)|subtype<br>void: none<br>ditstd: custom single<br>ditarr: custom arrayed<br>ditdld: download<br>dituld: upload<br>ditprg: progress|
srefsWznmMTag (string)|tag|
srefStdRefWznmMStub (string)|stub|
srefShoRefWznmMStub (string)|stub|
Avail (string)|availability rule|
Active (string)|activation rule|
srefsKOption (string)|options<br>bicol: bi-column<br>cap: capitalized title<br>ddd: title complement ' ...'<br>flexh: flexible height<br>icon: icon<br>iframe: inline frame<br>live: live data display<br>log: logarithmic scale<br>multsel: multiple item selection<br>mdnup: mouse down/up tracking<br>onoff: on and off states<br>rast: value raster<br>s: small<br>t: tall<br>tmstamp: time stamp scale<br>tmdate: date scale<br>tmtime: time scale<br>tricol: tri-column<br>xs: extra small|

[//]: # (IP ImeIMControl3.columns - END)

### 1.2.2.1 Parameters ``[ImeIAMControlPar3]``

[//]: # (IP ImeIAMControlPar3.superUse - BEGIN)

Super import: control (1:N)

Use:

[//]: # (IP ImeIAMControlPar3.superUse - END)

[//]: # (IP ImeIAMControlPar3.columns - BEGIN)

Column|Content|
-|-|
x1SrefKKey (string)|key<br>action: triggered action<br>cptwidth: caption width<br>height: height<br>icon: icon<br>stdicon: standard icon<br>width: width|
srefX2RefWznmMLocale (string)|locale|
osrefKVal (string)|value<br>crdopen: open card<br>dlgopen: open dialog<br>dlgclose: close dialog|

[//]: # (IP ImeIAMControlPar3.columns - END)

### 1.2.2.2 Stub by vector item ``[ImeIJMControl3]``

[//]: # (IP ImeIJMControl3.superUse - BEGIN)

Super import: control (1:N)

Use:

[//]: # (IP ImeIJMControl3.superUse - END)

[//]: # (IP ImeIJMControl3.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>retrupd: retrieve and update|
srefX1RefWznmMVectoritem (string)|vector item|
srefStdRefWznmMStub (string)|stub|
srefShoRefWznmMStub (string)|stub|

[//]: # (IP ImeIJMControl3.columns - END)

### 1.2.2.3 Name by locale ``[ImeIJMControlTitle3]``

[//]: # (IP ImeIJMControlTitle3.superUse - BEGIN)

Super import: control (1:N)

Use:

[//]: # (IP ImeIJMControlTitle3.superUse - END)

[//]: # (IP ImeIJMControlTitle3.columns - BEGIN)

Column|Content|
-|-|
srefX1RefWznmMLocale (string)|locale|
Title (string)|Title|

[//]: # (IP ImeIJMControlTitle3.columns - END)

### 1.2.2.4 Feed ``[ImeIMFeed3]``

[//]: # (IP ImeIMFeed3.superUse - BEGIN)

Super import: control (1:1)

Use:

[//]: # (IP ImeIMFeed3.superUse - END)

[//]: # (IP ImeIMFeed3.columns - BEGIN)

Column|Content|
-|-|
srefSrcIxVTbl (string)|source<br>void: none<br>vec: vector<br>tbl: table|
srefSrcUref (string)|source|
sref (string)|identifier|
srefsWznmMVectoritem (string)|vector item|
srefsWznmMTag (string)|tag|
Comment (string)|comment|

[//]: # (IP ImeIMFeed3.columns - END)

### 1.2.2.4.1 Vector ``[ImeIMVector3]``

[//]: # (IP ImeIMVector3.superUse - BEGIN)

Super import: feed (1:N)

Use:

[//]: # (IP ImeIMVector3.superUse - END)

[//]: # (IP ImeIMVector3.columns - BEGIN)

Column|Content|
-|-|
srefIxVBasetype (string)|type<br>lin: linear<br>or: multiple-choice<br>klst: key list<br>vlst: value list|
sref (string)|identifier|
osrefWznmKTaggrp (string)|source tag group<br>access: VecXxxxWAccess item<br>adrtype: address type<br>ctdet: contact detail<br>ctry: country<br>expstate: VecXxxxVExpstate item<br>iop: VecXxxxVIop item<br>lat: VecXxxxVLat item<br>lop: VecXxxxVLop item<br>mimetype: MIME type<br>no: no thing<br>none: none<br>oolop: VecXxxxVOolop item<br>prs: default person<br>prstit: person title<br>qrystate: VecXxxxVQrystate item<br>recaccess: VecXxxxVRecaccess item<br>reqitmode: VecXxxxVReqitmode item<br>sex: sex<br>start: login card<br>stdalr: standard alert message<br>stdrel: standard relation title<br>stdtbl: standard table title<br>stdtco: standard table column title<br>stdvec: standard vector title<br>uiaccess: VecXxxxWUiaccess item<br>userlevel: VecXxxxVUserlevel item<br>usrste: user state<br>wkday: weekday|
srefsKOption (string)|options<br>noloc: non-localized<br>notit: no titles<br>cmt: comments<br>apdfed: append to feed<br>filfed: fill feed|

[//]: # (IP ImeIMVector3.columns - END)

### 1.3 Panel ``[ImeIMPanel]``

[//]: # (IP ImeIMPanel.superUse - BEGIN)

Super import: card (1:N)

Use:

[//]: # (IP ImeIMPanel.superUse - END)

[//]: # (IP ImeIMPanel.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>retr: retrieve<br>retrupd: retrieve and update<br>rmv: remove|
srefIxVBasetype (string)|type<br>headbar: head bar<br>headline: headling line<br>form: form<br>list: list<br>rec: record<br>recform: form for record<br>reclist: list for record|
carNum (uint)|card|
sref (string)|identifier|
Detach (bool)|detachable|
Avail (string)|availability rule|
Comment (string)|comment|

[//]: # (IP ImeIMPanel.columns - END)

### 1.3.1 TblWznmCControl ``[ImeICControl2]``

[//]: # (IP ImeICControl2.superUse - BEGIN)

Super import: panel (1:N)

Use:

[//]: # (IP ImeICControl2.superUse - END)

[//]: # (IP ImeICControl2.columns - BEGIN)

Column|Content|
-|-|
iref (ubigint)|ref|

[//]: # (IP ImeICControl2.columns - END)

### 1.3.2 Control ``[ImeIMControl2]``

[//]: # (IP ImeIMControl2.superUse - BEGIN)

Super import: panel (1:N)

Use:

[//]: # (IP ImeIMControl2.superUse - END)

[//]: # (IP ImeIMControl2.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>retr: retrieve<br>retrupd: retrieve and update<br>rmv: remove|
iref (ubigint)|ref|
srefIxVBasetype (string)|type<br>alr: alert<br>but: button<br>chk: checkbox<br>cpt: caption<br>csi: color signal<br>cus: custom<br>dit: dialog item<br>dld: file download link<br>dse: dialog item selector<br>hdg: heading<br>hsb: horizontal scroll bar<br>lsb: list scroll bar<br>lst: list<br>mcb: multiple-choice button<br>men: menu<br>mit: menu item<br>msp: menu separator<br>mrl: URL menu item<br>mtx: menu item text display<br>pup: pop-up menu<br>rbu: radio button<br>sep: separator<br>sge: stage information<br>sld: slider<br>spc: spacer<br>tbl: table<br>tco: table column<br>tos: table order selector<br>trs: table row selector<br>tsb: table scroll bar<br>txf: text field<br>txt: text display<br>upd: up/down<br>uld: file upload field<br>vsb: vertical scroll bar|
irefRefWznmCControl (ubigint)|TblWznmCControl|
srefHkIxVSection (string)|hook<br>void: none<br>mbar: menu bar<br>side: side<br>hdr: header<br>hdrdetd: header when detached<br>hdrregd: header when regularized<br>cont: content<br>contdetd: content when detached<br>contregd: content when regularized<br>tbl: table<br>ftr: footer|
srefRefIxVTbl (string)|reference<br>void: none<br>dlg: dialog<br>qco: query column<br>rel: relation<br>tbl: table<br>tco: table column|
srefRefUref (string)|reference|
irefSupRefWznmMControl (ubigint)|super control|
srefIxVScope (string)|scope<br>app: app only<br>shr: shared app/engine|
sref (string)|identifier|
srefIxVSubtype (string)|subtype<br>void: none<br>ditstd: custom single<br>ditarr: custom arrayed<br>ditdld: download<br>dituld: upload<br>ditprg: progress|
srefsWznmMTag (string)|tag|
srefStdRefWznmMStub (string)|stub|
srefShoRefWznmMStub (string)|stub|
Avail (string)|availability rule|
Active (string)|activation rule|
srefsKOption (string)|options<br>bicol: bi-column<br>cap: capitalized title<br>ddd: title complement ' ...'<br>flexh: flexible height<br>icon: icon<br>iframe: inline frame<br>live: live data display<br>log: logarithmic scale<br>multsel: multiple item selection<br>mdnup: mouse down/up tracking<br>onoff: on and off states<br>rast: value raster<br>s: small<br>t: tall<br>tmstamp: time stamp scale<br>tmdate: date scale<br>tmtime: time scale<br>tricol: tri-column<br>xs: extra small|

[//]: # (IP ImeIMControl2.columns - END)

### 1.3.2.1 Parameters ``[ImeIAMControlPar2]``

[//]: # (IP ImeIAMControlPar2.superUse - BEGIN)

Super import: control (1:N)

Use:

[//]: # (IP ImeIAMControlPar2.superUse - END)

[//]: # (IP ImeIAMControlPar2.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>retrupd: retrieve and update|
x1SrefKKey (string)|key<br>action: triggered action<br>cptwidth: caption width<br>height: height<br>icon: icon<br>stdicon: standard icon<br>width: width|
srefX2RefWznmMLocale (string)|locale|
osrefKVal (string)|value<br>crdopen: open card<br>dlgopen: open dialog<br>dlgclose: close dialog|

[//]: # (IP ImeIAMControlPar2.columns - END)

### 1.3.2.2 Stub by vector item ``[ImeIJMControl2]``

[//]: # (IP ImeIJMControl2.superUse - BEGIN)

Super import: control (1:N)

Use:

[//]: # (IP ImeIJMControl2.superUse - END)

[//]: # (IP ImeIJMControl2.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>retrupd: retrieve and update|
srefX1RefWznmMVectoritem (string)|vector item|
srefStdRefWznmMStub (string)|stub|
srefShoRefWznmMStub (string)|stub|

[//]: # (IP ImeIJMControl2.columns - END)

### 1.3.2.3 Name by locale ``[ImeIJMControlTitle2]``

[//]: # (IP ImeIJMControlTitle2.superUse - BEGIN)

Super import: control (1:N)

Use:

[//]: # (IP ImeIJMControlTitle2.superUse - END)

[//]: # (IP ImeIJMControlTitle2.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>retrupd: retrieve and update|
srefX1RefWznmMLocale (string)|locale|
Title (string)|Title|

[//]: # (IP ImeIJMControlTitle2.columns - END)

### 1.3.2.4 Feed ``[ImeIMFeed2]``

[//]: # (IP ImeIMFeed2.superUse - BEGIN)

Super import: control (1:1)

Use:

[//]: # (IP ImeIMFeed2.superUse - END)

[//]: # (IP ImeIMFeed2.columns - BEGIN)

Column|Content|
-|-|
srefSrcIxVTbl (string)|source<br>void: none<br>vec: vector<br>tbl: table|
srefSrcUref (string)|source|
sref (string)|identifier|
srefsWznmMVectoritem (string)|vector item|
srefsWznmMTag (string)|tag|
Comment (string)|comment|

[//]: # (IP ImeIMFeed2.columns - END)

### 1.3.2.4.1 Vector ``[ImeIMVector2]``

[//]: # (IP ImeIMVector2.superUse - BEGIN)

Super import: feed (1:N)

Use:

[//]: # (IP ImeIMVector2.superUse - END)

[//]: # (IP ImeIMVector2.columns - BEGIN)

Column|Content|
-|-|
srefIxVBasetype (string)|type<br>lin: linear<br>or: multiple-choice<br>klst: key list<br>vlst: value list|
sref (string)|identifier|
osrefWznmKTaggrp (string)|source tag group<br>access: VecXxxxWAccess item<br>adrtype: address type<br>ctdet: contact detail<br>ctry: country<br>expstate: VecXxxxVExpstate item<br>iop: VecXxxxVIop item<br>lat: VecXxxxVLat item<br>lop: VecXxxxVLop item<br>mimetype: MIME type<br>no: no thing<br>none: none<br>oolop: VecXxxxVOolop item<br>prs: default person<br>prstit: person title<br>qrystate: VecXxxxVQrystate item<br>recaccess: VecXxxxVRecaccess item<br>reqitmode: VecXxxxVReqitmode item<br>sex: sex<br>start: login card<br>stdalr: standard alert message<br>stdrel: standard relation title<br>stdtbl: standard table title<br>stdtco: standard table column title<br>stdvec: standard vector title<br>uiaccess: VecXxxxWUiaccess item<br>userlevel: VecXxxxVUserlevel item<br>usrste: user state<br>wkday: weekday|
srefsKOption (string)|options<br>noloc: non-localized<br>notit: no titles<br>cmt: comments<br>apdfed: append to feed<br>filfed: fill feed|

[//]: # (IP ImeIMVector2.columns - END)

### 2 Presetting ``[ImeIMPreset]``

[//]: # (IP ImeIMPreset.superUse - BEGIN)

Use:

[//]: # (IP ImeIMPreset.superUse - END)

[//]: # (IP ImeIMPreset.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>rmv: remove|
srefRefIxVTbl (string)|reference<br>void: none<br>tbl: table<br>sbs: subset<br>vec: vector|
srefRefUref (string)|reference|
srefIxVScope (string)|scope<br>sys: system<br>sess: session<br>car: card<br>pnlrec: record panel<br>pnl: panel|
sref (string)|identifier|
srefIxWznmWArgtype (string)|argument type<br>ix: vector item index<br>ref: record reference<br>refs: set of record references<br>sref: string reference<br>intval: integer value<br>dblval: double value<br>boolval: boolean value<br>txtval: text value|

[//]: # (IP ImeIMPreset.columns - END)

### 2.1 Name by locale ``[ImeIJMPresetTitle]``

[//]: # (IP ImeIJMPresetTitle.superUse - BEGIN)

Super import: presetting (1:N)

Use:

[//]: # (IP ImeIJMPresetTitle.superUse - END)

[//]: # (IP ImeIJMPresetTitle.columns - BEGIN)

Column|Content|
-|-|
srefX1RefWznmMLocale (string)|locale|
Title (string)|Title|

[//]: # (IP ImeIJMPresetTitle.columns - END)

### 3 Query ``[ImeIMQuery]``

[//]: # (IP ImeIMQuery.superUse - BEGIN)

Use:

[//]: # (IP ImeIMQuery.superUse - END)

[//]: # (IP ImeIMQuery.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>retr: retrieve<br>retrupd: retrieve and update<br>rmv: remove|
iref (ubigint)|ref|
srefIxVBasetype (string)|type<br>std: standard<br>multbra: multi branch<br>list: list<br>oolist: operator ordered list|
irefSupRefWznmMQuery (ubigint)|super query|
srefSupIxVSubrole (string)|super query<br>void: none<br>opr: operator query<br>lref: list reference query|
sref (string)|identifier|
Limofs (bool)|Limofs|
Comment (string)|comment|

[//]: # (IP ImeIMQuery.columns - END)

### 3.1 Clauses ``[ImeIAMQueryClause]``

[//]: # (IP ImeIAMQueryClause.superUse - BEGIN)

Super import: query (1:N)

Use:

[//]: # (IP ImeIAMQueryClause.superUse - END)

[//]: # (IP ImeIAMQueryClause.columns - BEGIN)

Column|Content|
-|-|
irefX1RefWznmMQuerymod (ubigint)|query modifier|
srefIxVBasetype (string)|type<br>ix: custom index<br>ref: custom reference<br>eqn: equation<br>pre: presetting<br>vit: vector item<br>jref: job reference<br>lcl: locale<br>lat: list add type|
Clause (string)|clause|
srefRefWznmMPreset (string)|presetting|
srefRefWznmMVector (string)|vector|
srefRefWznmMVectoritem (string)|vector item|

[//]: # (IP ImeIAMQueryClause.columns - END)

### 3.2 Order rules ``[ImeIAMQueryOrder]``

[//]: # (IP ImeIAMQueryOrder.superUse - BEGIN)

Super import: query (1:N)

Use:

[//]: # (IP ImeIAMQueryOrder.superUse - END)

[//]: # (IP ImeIAMQueryOrder.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>rmv: remove|
Short (string)|acronym|
srefsWznmMTablecol (string)|table column|

[//]: # (IP ImeIAMQueryOrder.columns - END)

### 3.3 Query column ``[ImeIMQuerycol]``

[//]: # (IP ImeIMQuerycol.superUse - BEGIN)

Super import: query (1:N)

Use:

[//]: # (IP ImeIMQuerycol.superUse - END)

[//]: # (IP ImeIMQuerycol.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>retr: retrieve<br>retrupd: retrieve and update<br>rmv: remove|
srefIxVBasetype (string)|type<br>tbl: dual field in table<br>stub: stub to record<br>hstub: hierarchical stub to record<br>ustub: universal stub to record<br>stubs: stub to multi records<br>vsref: string ref to vector entry<br>vsrefs: string ref to multi vec entries<br>vtit: title to vector entry<br>vtits: titles to multi vector entries<br>yesno: yes/no of boolean<br>ftmdate: formatted date<br>ftmtime: formatted time<br>ftmstamp: formatted time stamp<br>ftmustamp: formatted time stamp with usecs<br>qidref: query table id ref<br>qwr: write flag<br>qjref: job ref<br>qjenum: job enumerator<br>intval: integer value<br>dblval: double value<br>boolval: boolean value<br>txtval: text value|
srefsIxWOccurrence (string)|occurrence<br>qtb: query table<br>xml: XML<br>btb: base table|
srefRefWznmMTablecol (string)|table column|
sref (string)|identifier|
Short (string)|acronym|
srefRefWznmMStub (string)|stub|

[//]: # (IP ImeIMQuerycol.columns - END)

### 3.3.1 Stub by presetting ``[ImeIJMQuerycolStub]``

[//]: # (IP ImeIJMQuerycolStub.superUse - BEGIN)

Super import: query column (1:N)

Use:

[//]: # (IP ImeIJMQuerycolStub.superUse - END)

[//]: # (IP ImeIJMQuerycolStub.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>retrupd: retrieve and update|
srefX1RefWznmMVectoritem (string)|vector item|
srefX2RefWznmMPreset (string)|presetting|
srefRefWznmMStub (string)|stub|

[//]: # (IP ImeIJMQuerycolStub.columns - END)

### 3.4 Query modifier ``[ImeIMQuerymod]``

[//]: # (IP ImeIMQuerymod.superUse - BEGIN)

Super import: query (1:N)

Use:

[//]: # (IP ImeIMQuerymod.superUse - END)

[//]: # (IP ImeIMQuerymod.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>retrupd: retrieve and update<br>rmv: remove|
iref (ubigint)|ref|
srefIxVBasetype (string)|type<br>bra: branch<br>exbra: exclusive branch<br>filt: filter<br>jovr: jump table override<br>stovr: sub1n/submn table override|
srefRefWznmMPreset (string)|presetting|
srefRefIxVTbl (string)|reference<br>void: none<br>axs: axis<br>tco: table column<br>tbl: table|
srefRefUref (string)|reference|
Avail (string)|availability rule|

[//]: # (IP ImeIMQuerymod.columns - END)

### 3.5 TblWznmRMQueryMTable ``[ImeIRMQueryMTable]``

[//]: # (IP ImeIRMQueryMTable.superUse - BEGIN)

Super import: query (1:N)

Use:

[//]: # (IP ImeIRMQueryMTable.superUse - END)

[//]: # (IP ImeIRMQueryMTable.columns - BEGIN)

Column|Content|
-|-|
srefRefWznmMTable (string)|table|
Source (bool)|Source|
Prefix (string)|prefix|

[//]: # (IP ImeIRMQueryMTable.columns - END)

### 3.5.1 TblWznmTMQuerymodMQuery ``[ImeITMQuerymodMQuery]``

[//]: # (IP ImeITMQuerymodMQuery.superUse - BEGIN)

Super import: TblWznmRMQueryMTable (1:N)

Use:

[//]: # (IP ImeITMQuerymodMQuery.superUse - END)

[//]: # (IP ImeITMQuerymodMQuery.columns - BEGIN)

Column|Content|
-|-|
irefRefWznmMQuerymod (ubigint)|query modifier|

[//]: # (IP ImeITMQuerymodMQuery.columns - END)

### 4 TblWznmRMPanelMQuery ``[ImeIRMPanelMQuery]``

[//]: # (IP ImeIRMPanelMQuery.superUse - BEGIN)

Use:

[//]: # (IP ImeIRMPanelMQuery.superUse - END)

[//]: # (IP ImeIRMPanelMQuery.columns - BEGIN)

Column|Content|
-|-|
srefRefWznmMPanel (string)|panel|
srefRefWznmMQuery (string)|query|

[//]: # (IP ImeIRMPanelMQuery.columns - END)

<em>Markdown for WhizniumSBE 0.9.12 auto-generated (what else ;-) ) by WhizniumSBE on 16 Sep 2018</em>