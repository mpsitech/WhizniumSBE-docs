Job tree ``[IexWznmJob]``
===

Schema
---

![](./IexWznmJob.jpg)

<p align="center"><em>Figure 1: Job tree schema - table columns in light blue are part of the input file, table columns in dark blue are inferred</em></p>

Structure
---

[//]: # (IP structure - BEGIN)

<br>&nbsp;&nbsp;&nbsp;&nbsp;\- Call listeners [``[ImeILstnRMCallMJob]``](#1-call-listeners-imeilstnrmcallmjob)
<br>&nbsp;&nbsp;&nbsp;&nbsp;\- Call [``[ImeIMCall]``](#2-call-imeimcall)
<br>&nbsp;&nbsp;&nbsp;&nbsp;\+ Job [``[ImeIMJob]``](#3-job-imeimjob)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Commands [``[ImeIAMJobCmd]``](#31-commands-imeiamjobcmd)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Variables [``[ImeIAMJobVar]``](#32-variables-imeiamjobvar)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Variables cluster [``[ImeICAMJobVar]``](#33-variables-cluster-imeicamjobvar)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Block [``[ImeIMBlock]``](#34-block-imeimblock)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Items [``[ImeIAMBlockItem]``](#341-items-imeiamblockitem)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Items cluster [``[ImeICAMBlockItem]``](#342-items-cluster-imeicamblockitem)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Method [``[ImeIMMethod]``](#35-method-imeimmethod)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Invocation parameters [``[ImeIAMMethodInvpar]``](#351-invocation-parameters-imeiammethodinvpar)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Return parameters [``[ImeIAMMethodRetpar]``](#352-return-parameters-imeiammethodretpar)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Stage [``[ImeIMStage]``](#36-stage-imeimstage)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Squawk [``[ImeIMSquawk]``](#361-squawk-imeimsquawk)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Text by locale [``[ImeIJMSquawkTitle]``](#3611-text-by-locale-imeijmsquawktitle)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Stubs [``[ImeIRMSquawkMStub]``](#3612-stubs-imeirmsquawkmstub)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Vector [``[ImeIMVector]``](#37-vector-imeimvector)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Vector item [``[ImeIMVectoritem]``](#371-vector-item-imeimvectoritem)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Name and comment by locale [``[ImeIJMVectoritem]``](#3711-name-and-comment-by-locale-imeijmvectoritem)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Operations [``[ImeIRMJobMOp]``](#38-operations-imeirmjobmop)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Operation packs [``[ImeIRMJobMOppack]``](#39-operation-packs-imeirmjobmoppack)
<br>&nbsp;&nbsp;&nbsp;&nbsp;\- Calls for stub updates [``[ImeIRMCallMStub]``](#4-calls-for-stub-updates-imeirmcallmstub)
<br>&nbsp;&nbsp;&nbsp;&nbsp;\- Job hierarchy [``[ImeIRMJobMJob]``](#5-job-hierarchy-imeirmjobmjob)

[//]: # (IP structure - END)

Details
---

### 1 Call listeners ``[ImeILstnRMCallMJob]``

[//]: # (IP ImeILstnRMCallMJob.superUse - BEGIN)

Use: which jobs listen to which calls.

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

Use: self-explanatory.

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

Use: retrieve auto-generated UI jobs, insert custom jobs.

[//]: # (IP ImeIMJob.superUse - END)

[//]: # (IP ImeIMJob.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>retr: retrieve|
sref (string)|identifier|
Mastslv (bool)|master/slave functionality|
Shrdat (bool)|shared data object between master and slaves|
Autostart (bool)|autostart|
Comment (string)|comment|

[//]: # (IP ImeIMJob.columns - END)

### 3.1 Commands ``[ImeIAMJobCmd]``

[//]: # (IP ImeIAMJobCmd.superUse - BEGIN)

Super import: job (1:N)

Use: command-line commands.

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

Use: variables, also available for M2M sessions.

[//]: # (IP ImeIAMJobVar.superUse - END)

[//]: # (IP ImeIAMJobVar.columns - BEGIN)

Column|Content|
-|-|
irefRefWznmCAMJobVar (ubigint)|integer reference to ImeICAMJobVar|
sref (string)|identifier|
srefIxWznmVVartype (string)|variable data type<br>void: none<br>boolean: boolean<br>tinyint: integer / byte (8bit)<br>utinyint: unsigned integer / byte (8bit)<br>smallint: integer (16bit)<br>usmallint: unsigned integer (16bit)<br>int: integer (32bit)<br>uint: unsigned integer (32bit)<br>bigint: integer (64bit)<br>ubigint: unsigned integer (64bit)<br>float: float<br>double: double<br>string: string<br>utinyintvec: unsigned int / byte 8bit vector<br>usmallintvec: unsigned int 16bit vector<br>intvec: integer 32bit vector<br>uintvec: unsigned int 32bit vector<br>ubigintvec: unsigned int 64bit vector<br>floatvec: float vector<br>doublevec: double vector<br>floatmat: float matrix<br>doublemat: double matrix<br>stringvec: string vector<br>vecsref: vector entry string reference<br>scrref: scrambled reference|
Shr (bool)|shared between master and slaves|
Comment (string)|comment|

[//]: # (IP ImeIAMJobVar.columns - END)

### 3.3 Variables cluster ``[ImeICAMJobVar]``

[//]: # (IP ImeICAMJobVar.superUse - BEGIN)

Super import: job (1:N)

Use: group variables.

[//]: # (IP ImeICAMJobVar.superUse - END)

[//]: # (IP ImeICAMJobVar.columns - BEGIN)

Column|Content|
-|-|
iref (ubigint)|integer reference|

[//]: # (IP ImeICAMJobVar.columns - END)

### 3.4 Block ``[ImeIMBlock]``

[//]: # (IP ImeIMBlock.superUse - BEGIN)

Super import: job (1:N)

Use: retrieve or insert data blocks.

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

Use: self-explanatory.

[//]: # (IP ImeIAMBlockItem.superUse - END)

[//]: # (IP ImeIAMBlockItem.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>retrupd: retrieve and update|
irefRefWznmCAMBlockItem (ubigint)|integer reference to ImeICAMBlockItem|
srefIxVBasetype (string)|type<br>var: standard variable<br>conpar: control parameter<br>contit: control title<br>feed: feed<br>rst: record set of query table<br>sub: sub-block|
sref (string)|identifier|
srefIxWznmVVartype (string)|variable data type<br>void: none<br>boolean: boolean<br>tinyint: integer / byte (8bit)<br>utinyint: unsigned integer / byte (8bit)<br>smallint: integer (16bit)<br>usmallint: unsigned integer (16bit)<br>int: integer (32bit)<br>uint: unsigned integer (32bit)<br>bigint: integer (64bit)<br>ubigint: unsigned integer (64bit)<br>float: float<br>double: double<br>string: string<br>utinyintvec: unsigned int / byte 8bit vector<br>usmallintvec: unsigned int 16bit vector<br>intvec: integer 32bit vector<br>uintvec: unsigned int 32bit vector<br>ubigintvec: unsigned int 64bit vector<br>floatvec: float vector<br>doublevec: double vector<br>floatmat: float matrix<br>doublemat: double matrix<br>stringvec: string vector<br>vecsref: vector entry string reference<br>scrref: scrambled reference|
srefRefWznmMControl (string)|conpar, contit types - control|
srefRefWznmMVector (string)|vecsref variable data type - vector|
srefRefWznmMFeed (string)|feed type - feed|
srefRefWznmMTable (string)|rst type - table|
srefRefWznmMBlock (string)|sub type - block|
Defval (string)|var type - default value|
srefRefWznmMVectoritem (string)|vecsref variable data type - vector item|
Comment (string)|comment|

[//]: # (IP ImeIAMBlockItem.columns - END)

### 3.4.2 Items cluster ``[ImeICAMBlockItem]``

[//]: # (IP ImeICAMBlockItem.superUse - BEGIN)

Super import: block (1:N)

Use: group block items.

[//]: # (IP ImeICAMBlockItem.superUse - END)

[//]: # (IP ImeICAMBlockItem.columns - BEGIN)

Column|Content|
-|-|
iref (ubigint)|ref|

[//]: # (IP ImeICAMBlockItem.columns - END)

### 3.5 Method ``[ImeIMMethod]``

[//]: # (IP ImeIMMethod.superUse - BEGIN)

Super import: job (1:N)

Use: methods, also available for M2M sessions.

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

Use: self-explanatory.

[//]: # (IP ImeIAMMethodInvpar.superUse - END)

[//]: # (IP ImeIAMMethodInvpar.columns - BEGIN)

Column|Content|
-|-|
sref (string)|identifier|
srefIxWznmVVartype (string)|variable data type<br>void: none<br>boolean: boolean<br>tinyint: integer / byte (8bit)<br>utinyint: unsigned integer / byte (8bit)<br>smallint: integer (16bit)<br>usmallint: unsigned integer (16bit)<br>int: integer (32bit)<br>uint: unsigned integer (32bit)<br>bigint: integer (64bit)<br>ubigint: unsigned integer (64bit)<br>float: float<br>double: double<br>string: string<br>utinyintvec: unsigned int / byte 8bit vector<br>usmallintvec: unsigned int 16bit vector<br>intvec: integer 32bit vector<br>uintvec: unsigned int 32bit vector<br>ubigintvec: unsigned int 64bit vector<br>floatvec: float vector<br>doublevec: double vector<br>floatmat: float matrix<br>doublemat: double matrix<br>stringvec: string vector<br>vecsref: vector entry string reference<br>scrref: scrambled reference|
srefRefWznmMVector (string)|vecsref variable data type - vector|
Comment (string)|comment|

[//]: # (IP ImeIAMMethodInvpar.columns - END)

### 3.5.2 Return parameters ``[ImeIAMMethodRetpar]``

[//]: # (IP ImeIAMMethodRetpar.superUse - BEGIN)

Super import: method (1:N)

Use: self-explanatory.

[//]: # (IP ImeIAMMethodRetpar.superUse - END)

[//]: # (IP ImeIAMMethodRetpar.columns - BEGIN)

Column|Content|
-|-|
sref (string)|identifier|
srefIxWznmVVartype (string)|variable data type<br>void: none<br>boolean: boolean<br>tinyint: integer / byte (8bit)<br>utinyint: unsigned integer / byte (8bit)<br>smallint: integer (16bit)<br>usmallint: unsigned integer (16bit)<br>int: integer (32bit)<br>uint: unsigned integer (32bit)<br>bigint: integer (64bit)<br>ubigint: unsigned integer (64bit)<br>float: float<br>double: double<br>string: string<br>utinyintvec: unsigned int / byte 8bit vector<br>usmallintvec: unsigned int 16bit vector<br>intvec: integer 32bit vector<br>uintvec: unsigned int 32bit vector<br>ubigintvec: unsigned int 64bit vector<br>floatvec: float vector<br>doublevec: double vector<br>floatmat: float matrix<br>doublemat: double matrix<br>stringvec: string vector<br>vecsref: vector entry string reference<br>scrref: scrambled reference|
srefRefWznmMVector (string)|vecsref variable data type - vector|
Comment (string)|comment|

[//]: # (IP ImeIAMMethodRetpar.columns - END)

### 3.6 Stage ``[ImeIMStage]``

[//]: # (IP ImeIMStage.superUse - BEGIN)

Super import: job (1:N)

Use: establish state machine for job.

[//]: # (IP ImeIMStage.superUse - END)

[//]: # (IP ImeIMStage.columns - BEGIN)

Column|Content|
-|-|
srefIxVBasetype (string)|type<br>opp: ops prepare<br>opiw: ops invoke and wait<br>oppiw: ops prepare, invoke and wait<br>alr: alert<br>immcb: immediate callback<br>other: other<br>othwc: other with wakeup call|
sref (string)|identifier|
srefIxVEnttype (string)|enter type<br>uld: on file upload<br>con: on control action<br>other: other|
esgSrefsWznmMStage (string)|stage from which to enter|
srefEcoRefWznmMControl (string)|control to enter|
Monitvl (uint)|monitor interval [µs]|
snxSrefWznmMStage (string)|next stage on success|
fnxSrefWznmMStage (string)|next stage on failure|
Comment (string)|comment|

[//]: # (IP ImeIMStage.columns - END)

### 3.6.1 Squawk ``[ImeIMSquawk]``

[//]: # (IP ImeIMSquawk.superUse - BEGIN)

Super import: stage (1:N)

Use: set human-readable status message during stage.

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

Use: self-explanatory.

[//]: # (IP ImeIJMSquawkTitle.superUse - END)

[//]: # (IP ImeIJMSquawkTitle.columns - BEGIN)

Column|Content|
-|-|
srefX1RefWznmMLocale (string)|locale|
Title (string)|string with placeholders|

[//]: # (IP ImeIJMSquawkTitle.columns - END)

### 3.6.1.2 Stubs ``[ImeIRMSquawkMStub]``

[//]: # (IP ImeIRMSquawkMStub.superUse - BEGIN)

Super import: squawk (1:N)

Use: define stubs included in squawk as placeholders.

[//]: # (IP ImeIRMSquawkMStub.superUse - END)

[//]: # (IP ImeIRMSquawkMStub.columns - BEGIN)

Column|Content|
-|-|
srefRefWznmMStub (string)|stub|

[//]: # (IP ImeIRMSquawkMStub.columns - END)

### 3.7 Vector ``[ImeIMVector]``

[//]: # (IP ImeIMVector.superUse - BEGIN)

Super import: job (1:N)

Use: job-specific vectors.

[//]: # (IP ImeIMVector.superUse - END)

[//]: # (IP ImeIMVector.columns - BEGIN)

Column|Content|
-|-|
srefIxWznmVIop (string)|import operation<br>ins: insert<br>retrupd: retrieve and update|
srefIxVBasetype (string)|type<br>lin: linear<br>or: multiple-choice|
sref (string)|identifier|
osrefWznmKTaggrp (string)|source tag group<br>access: VecXxxxWAccess item<br>adrtype: address type<br>ctdet: contact detail<br>ctry: country<br>expstate: VecXxxxVExpstate item<br>iop: VecXxxxVIop item<br>lat: VecXxxxVLat item<br>lop: VecXxxxVLop item<br>mimetype: MIME type<br>no: no thing<br>none: none<br>oolop: VecXxxxVOolop item<br>prs: default person<br>prstit: person title<br>qrystate: VecXxxxVQrystate item<br>recaccess: VecXxxxVRecaccess item<br>reqitmode: VecXxxxVReqitmode item<br>sex: sex<br>start: login card<br>stdalr: standard alert message<br>stdrel: standard relation title<br>stdtbl: standard table title<br>stdtco: standard table column title<br>stdvec: standard vector title<br>uiaccess: VecXxxxWUiaccess item<br>userlevel: VecXxxxVUserlevel item<br>usrste: user state<br>wkday: weekday|
srefsKOption (string)|options<br>noloc: non-localized<br>notit: no titles<br>cmt: comments<br>apdfed: append to feed<br>filfed: fill feed|

[//]: # (IP ImeIMVector.columns - END)

### 3.7.1 Vector item ``[ImeIMVectoritem]``

[//]: # (IP ImeIMVectoritem.superUse - BEGIN)

Super import: vector (1:N)

Use: self-explanatory.

[//]: # (IP ImeIMVectoritem.superUse - END)

[//]: # (IP ImeIMVectoritem.columns - BEGIN)

Column|Content|
-|-|
sref (string)|identifier|

[//]: # (IP ImeIMVectoritem.columns - END)

### 3.7.1.1 Name and comment by locale ``[ImeIJMVectoritem]``

[//]: # (IP ImeIJMVectoritem.superUse - BEGIN)

Super import: vector item (1:N)

Use: self-explanatory.

[//]: # (IP ImeIJMVectoritem.superUse - END)

[//]: # (IP ImeIJMVectoritem.columns - BEGIN)

Column|Content|
-|-|
srefX1RefWznmMLocale (string)|locale|
Title (string)|title|
Comment (string)|comment|

[//]: # (IP ImeIJMVectoritem.columns - END)

### 3.8 Operations ``[ImeIRMJobMOp]``

[//]: # (IP ImeIRMJobMOp.superUse - BEGIN)

Super import: job (1:N)

Use: operations the return dispatches of which are evaluated in the job.

[//]: # (IP ImeIRMJobMOp.superUse - END)

[//]: # (IP ImeIRMJobMOp.columns - BEGIN)

Column|Content|
-|-|
srefRefWznmMOp (string)|operation|

[//]: # (IP ImeIRMJobMOp.columns - END)

### 3.9 Operation packs ``[ImeIRMJobMOppack]``

[//]: # (IP ImeIRMJobMOppack.superUse - BEGIN)

Super import: job (1:N)

Use: customizable operation packs the return dispatches of which are evaluted in the job.

[//]: # (IP ImeIRMJobMOppack.superUse - END)

[//]: # (IP ImeIRMJobMOppack.columns - BEGIN)

Column|Content|
-|-|
srefRefWznmMOppack (string)|operation pack|

[//]: # (IP ImeIRMJobMOppack.columns - END)

### 4 Calls for stub updates ``[ImeIRMCallMStub]``

[//]: # (IP ImeIRMCallMStub.superUse - BEGIN)

Use: define which calls trigger which stub updates.

[//]: # (IP ImeIRMCallMStub.superUse - END)

[//]: # (IP ImeIRMCallMStub.columns - BEGIN)

Column|Content|
-|-|
srefRefWznmMCall (string)|call|
srefRefWznmMStub (string)|stub|

[//]: # (IP ImeIRMCallMStub.columns - END)

### 5 Job hierarchy ``[ImeIRMJobMJob]``

[//]: # (IP ImeIRMJobMJob.superUse - BEGIN)

Use: establish hierarchical structure of jobs.

[//]: # (IP ImeIRMJobMJob.superUse - END)

[//]: # (IP ImeIRMJobMJob.columns - BEGIN)

Column|Content|
-|-|
srefSupRefWznmMJob (string)|super job (#including sub-job)|
srefSubRefWznmMJob (string)|sub-job|
Short (string)|acronym|
Multi (bool)|multiple instances|
srefIxVInitype (string)|initialization type<br>void: none<br>cre: create<br>cremast: create as master<br>creslv: create as slave|

[//]: # (IP ImeIRMJobMJob.columns - END)

<em>Markdown for WhizniumSBE 0.9.12 auto-generated (what else ;-) ) by WhizniumSBE on 16 Sep 2018</em>
