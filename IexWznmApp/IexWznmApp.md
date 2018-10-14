App features ``[IexWznmApp]``
===

Schema
---

![](./IexWznmApp.jpg)

<p align="center"><em>Figure 1: App features schema - table columns in light blue are part of the input file, table columns in dark blue are inferred</em></p>

Structure
---

[//]: # (IP structure - BEGIN)

<br>&nbsp;&nbsp;&nbsp;&nbsp;\+ Run-time job [``[ImeIMRtjob]``](#1-run-time-job-imeimrtjob)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Run-time data block [``[ImeIMRtblock]``](#11-run-time-data-block-imeimrtblock)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Run-time dispatch [``[ImeIMRtdpch]``](#12-run-time-dispatch-imeimrtdpch)
<br>&nbsp;&nbsp;&nbsp;&nbsp;\+ Sequence [``[ImeIMSequence]``](#2-sequence-imeimsequence)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ State [``[ImeIMState]``](#21-state-imeimstate)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Steppings [``[ImeIAMStateStep]``](#211-steppings-imeiamstatestep)

[//]: # (IP structure - END)

Details
---

### 1 Run-time job ``[ImeIMRtjob]``

[//]: # (IP ImeIMRtjob.superUse - BEGIN)

Use: specify the part of job tree which is relevant for the app / establish hierarchical DOM.

[//]: # (IP ImeIMRtjob.superUse - END)

[//]: # (IP ImeIMRtjob.columns - BEGIN)

Column|Content|
-|-|
iref (ubigint)|integer reference|
irefSupRefWznmMRtjob (ubigint)|super run-time job|
srefRefWznmMJob (string)|job|
sref (string)|identifier|
Comment (string)|comment|

[//]: # (IP ImeIMRtjob.columns - END)

### 1.1 Run-time data block ``[ImeIMRtblock]``

[//]: # (IP ImeIMRtblock.superUse - BEGIN)

Super import: run-time job (1:N)

Use: specify XML data blocks relevant for the app, to be incorporated into the DOM.

[//]: # (IP ImeIMRtblock.superUse - END)

[//]: # (IP ImeIMRtblock.columns - BEGIN)

Column|Content|
-|-|
srefRefIxVTbl (string)|reference<br>blk: block<br>fed: feed<br>tbl: table|
srefRefUref (string)|reference|
sref (string)|identifier|
srcSrefsWznmAMBlockItem (string)|dispatch sources|

[//]: # (IP ImeIMRtblock.columns - END)

### 1.2 Run-time dispatch ``[ImeIMRtdpch]``

[//]: # (IP ImeIMRtdpch.superUse - BEGIN)

Super import: run-time job (1:N)

Use: engine dispatches to be processed in the app.

[//]: # (IP ImeIMRtdpch.superUse - END)

[//]: # (IP ImeIMRtdpch.columns - BEGIN)

Column|Content|
-|-|
srefRefWznmMBlock (string)|dispatch|
sref (string)|identifier|
Merge (bool)|merge content|

[//]: # (IP ImeIMRtdpch.columns - END)

### 2 Sequence ``[ImeIMSequence]``

[//]: # (IP ImeIMSequence.superUse - BEGIN)

Use: grouping entity for states.

[//]: # (IP ImeIMSequence.superUse - END)

[//]: # (IP ImeIMSequence.columns - BEGIN)

Column|Content|
-|-|
sref (string)|identifier|
Title (string)|title|
Comment (string)|comment|

[//]: # (IP ImeIMSequence.columns - END)

### 2.1 State ``[ImeIMState]``

[//]: # (IP ImeIMState.superUse - BEGIN)

Super import: sequence (1:N)

Use: state machine definition, allowing to perform several dispatch exchanges with the engine in a row, in event-driven fashion.

[//]: # (IP ImeIMState.superUse - END)

[//]: # (IP ImeIMState.columns - BEGIN)

Column|Content|
-|-|
sref (string)|identifier|
srefEacIxVAction (string)|action when entering<br>void: none<br>login: start session<br>init: initialize UI job<br>do: trigger UI action<br>step: step to next state<br>cust: custom code|
irefErjRefWznmMRtjob (ubigint)|run-time job for enter action|
srefEveRefWznmMVector (string)|do vector for enter action|
srefEviRefWznmMVectoritem (string)|do vector item for enter action|
srefEsnRefWznmMState (string)|state to step to for enter action|
srefLacIxVAction (string)|action when leaving<br>void: none<br>login: start session<br>init: initialize UI job<br>do: trigger UI action<br>step: step to next state<br>cust: custom code|
Custstep (bool)|custom code insertion point for stepping|
Comment (string)|comment|

[//]: # (IP ImeIMState.columns - END)

### 2.1.1 Steppings ``[ImeIAMStateStep]``

[//]: # (IP ImeIAMStateStep.superUse - BEGIN)

Super import: state (1:N)

Use: conditional change of state.

[//]: # (IP ImeIAMStateStep.superUse - END)

[//]: # (IP ImeIAMStateStep.columns - BEGIN)

Column|Content|
-|-|
srefSnxRefWznmMState (string)|next state|
srefIxVTrigger (string)|trigger<br>sgeeq: stage equals<br>jobex: job exists<br>jobnex: job doesn't exist<br>confacc: confirmation received<br>confdny: denial received<br>dpchrcv: dispatch received<br>cust: custom condition|
irefRefWznmMRtjob (ubigint)|jobex, jobnex, confacc, confdny, dpchrcv triggers - run-time job concerned|
srefRefWznmMVectoritem (string)|vector item|
xsref (string)|confacc trigger - sref (identifier) content filter|
srefRefWznmMRtdpch (string)|dpchrcv trigger - run-time dispatch|
srefsMask (string)|dpchrcv trigger - mandatory content of dispatch received|
Cond (string)|cust trigger - condition (actual C++/Objective-C/Java code)|
Custcode (bool)|custom code insertion point|

[//]: # (IP ImeIAMStateStep.columns - END)

<em>Markdown for WhizniumSBE 0.9.12 auto-generated (what else ;-) ) by WhizniumSBE on 16 Sep 2018</em>
