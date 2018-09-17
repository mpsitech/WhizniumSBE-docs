Job tree ``[IexWznmJob]``
===

Schema
---

![](./IexWznmJob.jpg)

<p align="center"><em>Figure 1: Job tree schema - table columns in light blue are part of the input file, table columns in dark blue are inferred</em></p>

Structure
---

[//]: # (IP structure - BEGIN)

<br>&nbsp;&nbsp;&nbsp;&nbsp;\- TblWznmLstnRMCallMJob [``[ImeILstnRMCallMJob]``](#1-tblwznmlstnrmcallmjob-imeilstnrmcallmjob)
<br>&nbsp;&nbsp;&nbsp;&nbsp;\- Call [``[ImeIMCall]``](#2-call-imeimcall)
<br>&nbsp;&nbsp;&nbsp;&nbsp;\+ Job [``[ImeIMJob]``](#3-job-imeimjob)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Commands [``[ImeIAMJobCmd]``](#31-commands-imeiamjobcmd)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Variables [``[ImeIAMJobVar]``](#32-variables-imeiamjobvar)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- TblWznmCAMJobVar [``[ImeICAMJobVar]``](#33-tblwznmcamjobvar-imeicamjobvar)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Block [``[ImeIMBlock]``](#34-block-imeimblock)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Items [``[ImeIAMBlockItem]``](#341-items-imeiamblockitem)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- TblWznmCAMBlockItem [``[ImeICAMBlockItem]``](#342-tblwznmcamblockitem-imeicamblockitem)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Method [``[ImeIMMethod]``](#35-method-imeimmethod)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Invocation parameters [``[ImeIAMMethodInvpar]``](#351-invocation-parameters-imeiammethodinvpar)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Return parameters [``[ImeIAMMethodRetpar]``](#352-return-parameters-imeiammethodretpar)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Stage [``[ImeIMStage]``](#36-stage-imeimstage)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Squawk [``[ImeIMSquawk]``](#361-squawk-imeimsquawk)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Text by locale [``[ImeIJMSquawkTitle]``](#3611-text-by-locale-imeijmsquawktitle)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- TblWznmRMSquawkMStub [``[ImeIRMSquawkMStub]``](#3612-tblwznmrmsquawkmstub-imeirmsquawkmstub)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Vector [``[ImeIMVector]``](#37-vector-imeimvector)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Vector item [``[ImeIMVectoritem]``](#371-vector-item-imeimvectoritem)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Name and comment by locale [``[ImeIJMVectoritem]``](#3711-name-and-comment-by-locale-imeijmvectoritem)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- TblWznmRMJobMOp [``[ImeIRMJobMOp]``](#38-tblwznmrmjobmop-imeirmjobmop)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- TblWznmRMJobMOppack [``[ImeIRMJobMOppack]``](#39-tblwznmrmjobmoppack-imeirmjobmoppack)
<br>&nbsp;&nbsp;&nbsp;&nbsp;\- TblWznmRMCallMStub [``[ImeIRMCallMStub]``](#4-tblwznmrmcallmstub-imeirmcallmstub)
<br>&nbsp;&nbsp;&nbsp;&nbsp;\- TblWznmRMJobMJob [``[ImeIRMJobMJob]``](#5-tblwznmrmjobmjob-imeirmjobmjob)

[//]: # (IP structure - END)

Details
---

### 1 TblWznmLstnRMCallMJob ``[ImeILstnRMCallMJob]``

[//]: # (IP ImeILstnRMCallMJob.superUse - BEGIN)

Use:

[//]: # (IP ImeILstnRMCallMJob.superUse - END)

[//]: # (IP ImeILstnRMCallMJob.columns - BEGIN)

Column|Content|
-|-|
srefRefWznmMCall (string)|call|
srefRefWznmMJob (string)|job|
srefIxVJobmask (string)|job mask<br>all: all jobs<br>imm: immediate sub-jobs<br>mast: master job<br>self: same job<br>slv: slave jobs<br>spec: specific job<br>tree: tree of sub-jobs|
srefsAmsIxWznmWArgtype (string)|argument mask<br>ix: vector item index<br>ref: record reference<br>refs: set of record references<br>sref: string reference<br>intval: integer value<br>dblval: double value<br>boolval: boolean value<br>txtval: text value|
srefIxVJactype (string)|job access type<br>lock: mutex lock<br>try: try mutex lock<br>weak: no mutex lock|

[//]: # (IP ImeILstnRMCallMJob.columns - END)

### 2 Call ``[ImeIMCall]``

[//]: # (IP ImeIMCall.superUse - BEGIN)

Use:

[//]: # (IP ImeIMCall.superUse - END)

[//]: # (IP ImeIMCall.columns - BEGIN)

Column|Content|
-|-|
srefIxVBasetype (string)|type<br>chk: record feature check<br>evt: other event<br>pstset: presetting set request<br>recupd: record update event<br>tblmod: table modification event<br>other: other|
srefsInvIxWznmWArgtype (string)|invocation argument types<br>ix: vector item index<br>ref: record reference<br>refs: set of record references<br>sref: string reference<br>intval: integer value<br>dblval: double value<br>boolval: boolean value<br>txtval: text value|
srefsRetIxWznmWArgtype (string)|return argument types<br>ix: vector item index<br>ref: record reference<br>refs: set of record references<br>sref: string reference<br>intval: integer value<br>dblval: double value<br>boolval: boolean value<br>txtval: text value|
sref (string)|identifier|
Comment (string)|comment|

[//]: # (IP ImeIMCall.columns - END)

### 3 Job ``[ImeIMJob]``

[//]: # (IP ImeIMJob.superUse - BEGIN)

Use:

[//]: # (IP ImeIMJob.superUse - END)

[//]: # (IP ImeIMJob.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>retr: retrieve|
sref (string)|identifier|
Mastslv (bool)|master/slave|
Shrdat (bool)|shared data|
Autostart (bool)|autostart|
Comment (string)|comment|

[//]: # (IP ImeIMJob.columns - END)

### 3.1 Commands ``[ImeIAMJobCmd]``

[//]: # (IP ImeIAMJobCmd.superUse - BEGIN)

Super import: job (1:N)

Use:

[//]: # (IP ImeIAMJobCmd.superUse - END)

[//]: # (IP ImeIAMJobCmd.columns - BEGIN)

Column|Content|
-|-|
sref (string)|identifier|
Comment (string)|comment|

[//]: # (IP ImeIAMJobCmd.columns - END)

### 3.2 Variables ``[ImeIAMJobVar]``

[//]: # (IP ImeIAMJobVar.superUse - BEGIN)

Super import: job (1:N)

Use:

[//]: # (IP ImeIAMJobVar.superUse - END)

[//]: # (IP ImeIAMJobVar.columns - BEGIN)

Column|Content|
-|-|
irefRefWznmCAMJobVar (ubigint)|TblWznmCAMJobVar|
sref (string)|identifier|
srefIxWznmVVartype (string)|variable data type<br>void: none<br>boolean: boolean<br>tinyint: integer / byte (8bit)<br>utinyint: unsigned integer / byte (8bit)<br>smallint: integer (16bit)<br>usmallint: unsigned integer (16bit)<br>int: integer (32bit)<br>uint: unsigned integer (32bit)<br>bigint: integer (64bit)<br>ubigint: unsigned integer (64bit)<br>float: float<br>double: double<br>string: string<br>utinyintvec: unsigned int / byte 8bit vector<br>usmallintvec: unsigned int 16bit vector<br>intvec: integer 32bit vector<br>uintvec: unsigned int 32bit vector<br>ubigintvec: unsigned int 64bit vector<br>floatvec: float vector<br>doublevec: double vector<br>floatmat: float matrix<br>doublemat: double matrix<br>stringvec: string vector<br>vecsref: vector entry string reference<br>scrref: scrambled reference|
Shr (bool)|shared|
Comment (string)|comment|

[//]: # (IP ImeIAMJobVar.columns - END)

### 3.3 TblWznmCAMJobVar ``[ImeICAMJobVar]``

[//]: # (IP ImeICAMJobVar.superUse - BEGIN)

Super import: job (1:N)

Use:

[//]: # (IP ImeICAMJobVar.superUse - END)

[//]: # (IP ImeICAMJobVar.columns - BEGIN)

Column|Content|
-|-|
iref (ubigint)|ref|

[//]: # (IP ImeICAMJobVar.columns - END)

### 3.4 Block ``[ImeIMBlock]``

[//]: # (IP ImeIMBlock.superUse - BEGIN)

Super import: job (1:N)

Use:

[//]: # (IP ImeIMBlock.superUse - END)

[//]: # (IP ImeIMBlock.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>retr: retrieve<br>retrupd: retrieve and update|
srefIxVBasetype (string)|type<br>cont: form content<br>dpch: dispatch<br>stat: state list<br>stg: setting list<br>tag: tag list|
srefsReaIxWznmWScope (string)|read scope<br>app: app<br>cmbeng: combined engine<br>eng: main engine<br>openg: operation engine|
srefsWriIxWznmWScope (string)|write scope<br>app: app<br>cmbeng: combined engine<br>eng: main engine<br>openg: operation engine|
sref (string)|identifier|
Comment (string)|comment|

[//]: # (IP ImeIMBlock.columns - END)

### 3.4.1 Items ``[ImeIAMBlockItem]``

[//]: # (IP ImeIAMBlockItem.superUse - BEGIN)

Super import: block (1:N)

Use:

[//]: # (IP ImeIAMBlockItem.superUse - END)

[//]: # (IP ImeIAMBlockItem.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>retrupd: retrieve and update|
irefRefWznmCAMBlockItem (ubigint)|TblWznmCAMBlockItem|
srefIxVBasetype (string)|type<br>var: standard variable<br>conpar: control parameter<br>contit: control title<br>feed: feed<br>rst: record set of query table<br>sub: sub-block|
sref (string)|identifier|
srefIxWznmVVartype (string)|variable data type<br>void: none<br>boolean: boolean<br>tinyint: integer / byte (8bit)<br>utinyint: unsigned integer / byte (8bit)<br>smallint: integer (16bit)<br>usmallint: unsigned integer (16bit)<br>int: integer (32bit)<br>uint: unsigned integer (32bit)<br>bigint: integer (64bit)<br>ubigint: unsigned integer (64bit)<br>float: float<br>double: double<br>string: string<br>utinyintvec: unsigned int / byte 8bit vector<br>usmallintvec: unsigned int 16bit vector<br>intvec: integer 32bit vector<br>uintvec: unsigned int 32bit vector<br>ubigintvec: unsigned int 64bit vector<br>floatvec: float vector<br>doublevec: double vector<br>floatmat: float matrix<br>doublemat: double matrix<br>stringvec: string vector<br>vecsref: vector entry string reference<br>scrref: scrambled reference|
srefRefWznmMControl (string)|control|
srefRefWznmMVector (string)|vector|
srefRefWznmMFeed (string)|feed|
srefRefWznmMTable (string)|table|
srefRefWznmMBlock (string)|block|
Defval (string)|default value|
srefRefWznmMVectoritem (string)|vector item|
Comment (string)|comment|

[//]: # (IP ImeIAMBlockItem.columns - END)

### 3.4.2 TblWznmCAMBlockItem ``[ImeICAMBlockItem]``

[//]: # (IP ImeICAMBlockItem.superUse - BEGIN)

Super import: block (1:N)

Use:

[//]: # (IP ImeICAMBlockItem.superUse - END)

[//]: # (IP ImeICAMBlockItem.columns - BEGIN)

Column|Content|
-|-|
iref (ubigint)|ref|

[//]: # (IP ImeICAMBlockItem.columns - END)

### 3.5 Method ``[ImeIMMethod]``

[//]: # (IP ImeIMMethod.superUse - BEGIN)

Super import: job (1:N)

Use:

[//]: # (IP ImeIMMethod.superUse - END)

[//]: # (IP ImeIMMethod.columns - BEGIN)

Column|Content|
-|-|
sref (string)|identifier|
Execmast (bool)|execute as master|
Comment (string)|comment|

[//]: # (IP ImeIMMethod.columns - END)

### 3.5.1 Invocation parameters ``[ImeIAMMethodInvpar]``

[//]: # (IP ImeIAMMethodInvpar.superUse - BEGIN)

Super import: method (1:N)

Use:

[//]: # (IP ImeIAMMethodInvpar.superUse - END)

[//]: # (IP ImeIAMMethodInvpar.columns - BEGIN)

Column|Content|
-|-|
sref (string)|identifier|
srefIxWznmVVartype (string)|variable data type<br>void: none<br>boolean: boolean<br>tinyint: integer / byte (8bit)<br>utinyint: unsigned integer / byte (8bit)<br>smallint: integer (16bit)<br>usmallint: unsigned integer (16bit)<br>int: integer (32bit)<br>uint: unsigned integer (32bit)<br>bigint: integer (64bit)<br>ubigint: unsigned integer (64bit)<br>float: float<br>double: double<br>string: string<br>utinyintvec: unsigned int / byte 8bit vector<br>usmallintvec: unsigned int 16bit vector<br>intvec: integer 32bit vector<br>uintvec: unsigned int 32bit vector<br>ubigintvec: unsigned int 64bit vector<br>floatvec: float vector<br>doublevec: double vector<br>floatmat: float matrix<br>doublemat: double matrix<br>stringvec: string vector<br>vecsref: vector entry string reference<br>scrref: scrambled reference|
srefRefWznmMVector (string)|vector|
Comment (string)|comment|

[//]: # (IP ImeIAMMethodInvpar.columns - END)

### 3.5.2 Return parameters ``[ImeIAMMethodRetpar]``

[//]: # (IP ImeIAMMethodRetpar.superUse - BEGIN)

Super import: method (1:N)

Use:

[//]: # (IP ImeIAMMethodRetpar.superUse - END)

[//]: # (IP ImeIAMMethodRetpar.columns - BEGIN)

Column|Content|
-|-|
sref (string)|identifier|
srefIxWznmVVartype (string)|variable data type<br>void: none<br>boolean: boolean<br>tinyint: integer / byte (8bit)<br>utinyint: unsigned integer / byte (8bit)<br>smallint: integer (16bit)<br>usmallint: unsigned integer (16bit)<br>int: integer (32bit)<br>uint: unsigned integer (32bit)<br>bigint: integer (64bit)<br>ubigint: unsigned integer (64bit)<br>float: float<br>double: double<br>string: string<br>utinyintvec: unsigned int / byte 8bit vector<br>usmallintvec: unsigned int 16bit vector<br>intvec: integer 32bit vector<br>uintvec: unsigned int 32bit vector<br>ubigintvec: unsigned int 64bit vector<br>floatvec: float vector<br>doublevec: double vector<br>floatmat: float matrix<br>doublemat: double matrix<br>stringvec: string vector<br>vecsref: vector entry string reference<br>scrref: scrambled reference|
srefRefWznmMVector (string)|vector|
Comment (string)|comment|

[//]: # (IP ImeIAMMethodRetpar.columns - END)

### 3.6 Stage ``[ImeIMStage]``

[//]: # (IP ImeIMStage.superUse - BEGIN)

Super import: job (1:N)

Use:

[//]: # (IP ImeIMStage.superUse - END)

[//]: # (IP ImeIMStage.columns - BEGIN)

Column|Content|
-|-|
srefIxVBasetype (string)|type<br>opp: ops prepare<br>opiw: ops invoke and wait<br>oppiw: ops prepare, invoke and wait<br>alr: alert<br>immcb: immediate callback<br>other: other<br>othwc: other with wakeup call|
sref (string)|identifier|
srefIxVEnttype (string)|enter type<br>uld: on file upload<br>con: on control action<br>other: other|
esgSrefsWznmMStage (string)|stage|
srefEcoRefWznmMControl (string)|control to enter|
Monitvl (uint)|monitor interval [\u00b5s]|
snxSrefWznmMStage (string)|next stage on success|
fnxSrefWznmMStage (string)|next stage on failure|
Comment (string)|comment|

[//]: # (IP ImeIMStage.columns - END)

### 3.6.1 Squawk ``[ImeIMSquawk]``

[//]: # (IP ImeIMSquawk.superUse - BEGIN)

Super import: stage (1:N)

Use:

[//]: # (IP ImeIMSquawk.superUse - END)

[//]: # (IP ImeIMSquawk.columns - BEGIN)

Column|Content|
-|-|
sref (string)|identifier|
Example (string)|example|

[//]: # (IP ImeIMSquawk.columns - END)

### 3.6.1.1 Text by locale ``[ImeIJMSquawkTitle]``

[//]: # (IP ImeIJMSquawkTitle.superUse - BEGIN)

Super import: squawk (1:N)

Use:

[//]: # (IP ImeIJMSquawkTitle.superUse - END)

[//]: # (IP ImeIJMSquawkTitle.columns - BEGIN)

Column|Content|
-|-|
srefX1RefWznmMLocale (string)|locale|
Title (string)|Title|

[//]: # (IP ImeIJMSquawkTitle.columns - END)

### 3.6.1.2 TblWznmRMSquawkMStub ``[ImeIRMSquawkMStub]``

[//]: # (IP ImeIRMSquawkMStub.superUse - BEGIN)

Super import: squawk (1:N)

Use:

[//]: # (IP ImeIRMSquawkMStub.superUse - END)

[//]: # (IP ImeIRMSquawkMStub.columns - BEGIN)

Column|Content|
-|-|
srefRefWznmMStub (string)|stub|

[//]: # (IP ImeIRMSquawkMStub.columns - END)

### 3.7 Vector ``[ImeIMVector]``

[//]: # (IP ImeIMVector.superUse - BEGIN)

Super import: job (1:N)

Use:

[//]: # (IP ImeIMVector.superUse - END)

[//]: # (IP ImeIMVector.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>retrupd: retrieve and update|
srefIxVBasetype (string)|type<br>lin: linear<br>or: multiple-choice<br>klst: key list<br>vlst: value list|
sref (string)|identifier|
osrefWznmKTaggrp (string)|source tag group<br>access: VecXxxxWAccess item<br>adrtype: address type<br>ctdet: contact detail<br>ctry: country<br>expstate: VecXxxxVExpstate item<br>iop: VecXxxxVIop item<br>lat: VecXxxxVLat item<br>lop: VecXxxxVLop item<br>mimetype: MIME type<br>no: no thing<br>none: none<br>oolop: VecXxxxVOolop item<br>prs: default person<br>prstit: person title<br>qrystate: VecXxxxVQrystate item<br>recaccess: VecXxxxVRecaccess item<br>reqitmode: VecXxxxVReqitmode item<br>sex: sex<br>start: login card<br>stdalr: standard alert message<br>stdrel: standard relation title<br>stdtbl: standard table title<br>stdtco: standard table column title<br>stdvec: standard vector title<br>uiaccess: VecXxxxWUiaccess item<br>userlevel: VecXxxxVUserlevel item<br>usrste: user state<br>wkday: weekday|
srefsKOption (string)|options<br>noloc: non-localized<br>notit: no titles<br>cmt: comments<br>apdfed: append to feed<br>filfed: fill feed|

[//]: # (IP ImeIMVector.columns - END)

### 3.7.1 Vector item ``[ImeIMVectoritem]``

[//]: # (IP ImeIMVectoritem.superUse - BEGIN)

Super import: vector (1:N)

Use:

[//]: # (IP ImeIMVectoritem.superUse - END)

[//]: # (IP ImeIMVectoritem.columns - BEGIN)

Column|Content|
-|-|
sref (string)|identifier|

[//]: # (IP ImeIMVectoritem.columns - END)

### 3.7.1.1 Name and comment by locale ``[ImeIJMVectoritem]``

[//]: # (IP ImeIJMVectoritem.superUse - BEGIN)

Super import: vector item (1:N)

Use:

[//]: # (IP ImeIJMVectoritem.superUse - END)

[//]: # (IP ImeIJMVectoritem.columns - BEGIN)

Column|Content|
-|-|
srefX1RefWznmMLocale (string)|locale|
Title (string)|Title|
Comment (string)|Comment|

[//]: # (IP ImeIJMVectoritem.columns - END)

### 3.8 TblWznmRMJobMOp ``[ImeIRMJobMOp]``

[//]: # (IP ImeIRMJobMOp.superUse - BEGIN)

Super import: job (1:N)

Use:

[//]: # (IP ImeIRMJobMOp.superUse - END)

[//]: # (IP ImeIRMJobMOp.columns - BEGIN)

Column|Content|
-|-|
srefRefWznmMOp (string)|operation|

[//]: # (IP ImeIRMJobMOp.columns - END)

### 3.9 TblWznmRMJobMOppack ``[ImeIRMJobMOppack]``

[//]: # (IP ImeIRMJobMOppack.superUse - BEGIN)

Super import: job (1:N)

Use:

[//]: # (IP ImeIRMJobMOppack.superUse - END)

[//]: # (IP ImeIRMJobMOppack.columns - BEGIN)

Column|Content|
-|-|
srefRefWznmMOppack (string)|operation pack|

[//]: # (IP ImeIRMJobMOppack.columns - END)

### 4 TblWznmRMCallMStub ``[ImeIRMCallMStub]``

[//]: # (IP ImeIRMCallMStub.superUse - BEGIN)

Use:

[//]: # (IP ImeIRMCallMStub.superUse - END)

[//]: # (IP ImeIRMCallMStub.columns - BEGIN)

Column|Content|
-|-|
srefRefWznmMCall (string)|call|
srefRefWznmMStub (string)|stub|

[//]: # (IP ImeIRMCallMStub.columns - END)

### 5 TblWznmRMJobMJob ``[ImeIRMJobMJob]``

[//]: # (IP ImeIRMJobMJob.superUse - BEGIN)

Use:

[//]: # (IP ImeIRMJobMJob.superUse - END)

[//]: # (IP ImeIRMJobMJob.columns - BEGIN)

Column|Content|
-|-|
srefSupRefWznmMJob (string)|job|
srefSubRefWznmMJob (string)|job|
Short (string)|acronym|
Multi (bool)|multi|
srefIxVInitype (string)|initialization type<br>void: none<br>cre: create<br>cremast: create as master<br>creslv: create as slave|

[//]: # (IP ImeIRMJobMJob.columns - END)

<em>Markdown for WhizniumSBE 0.9.12 auto-generated (what else ;-) ) by WhizniumSBE on 16 Sep 2018</em>
