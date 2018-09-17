Database structure ``[IexWznmDbs]``
===

Schema
---

![Figure 1: Database structure schema - table columns in light blue are part of the input file, table columns in dark blue are inferred](./IexWznmDbs.jpg)

Structure
---

[//]: # (IP structure - BEGIN)

<br>&nbsp;&nbsp;&nbsp;&nbsp;\- TblWznmCRelation [``[ImeICRelation]``](#1-tblwznmcrelation-imeicrelation)
<br>&nbsp;&nbsp;&nbsp;&nbsp;\+ Relation [``[ImeIMRelation]``](#ImeIMRelation)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Names [``[ImeIAMRelationTitle]``](#ImeIAMRelationTitle)
<br>&nbsp;&nbsp;&nbsp;&nbsp;\- Stub [``[ImeIMStub]``](#ImeIMStub)
<br>&nbsp;&nbsp;&nbsp;&nbsp;\+ Table [``[ImeIMTable]``](#ImeIMTable)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Load functions [``[ImeIAMTableLoadfct]``](#ImeIAMTableLoadfct)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Names [``[ImeIAMTableTitle]``](#ImeIAMTableTitle)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Feature check [``[ImeIMCheck]``](#ImeIMCheck)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Subset [``[ImeIMSubset]``](#ImeIMSubset)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Names [``[ImeIAMSubsetTitle]``](#ImeIAMSubsetTitle)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- TblWznmRMSubsetMSubset [``[ImeIRMSubsetMSubset]``](#ImeIRMSubsetMSubset)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Table column [``[ImeIMTablecol]``](#ImeIMTablecol)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Names [``[ImeIAMTablecolTitle]``](#ImeIAMTablecolTitle)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Vector [``[ImeIMVector2]``](#ImeIMVector2)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Names [``[ImeIAMVectorTitle2]``](#ImeIAMVectorTitle2)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Vector item [``[ImeIMVectoritem2]``](#ImeIMVectoritem2)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Name and comment by locale [``[ImeIJMVectoritem2]``](#ImeIJMVectoritem2)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- TblWznmRMTableMVector [``[ImeIRMTableMVector2]``](#ImeIRMTableMVector2)
<br>&nbsp;&nbsp;&nbsp;&nbsp;\+ Vector [``[ImeIMVector1]``](#ImeIMVector1)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Names [``[ImeIAMVectorTitle1]``](#ImeIAMVectorTitle1)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\+ Vector item [``[ImeIMVectoritem1]``](#ImeIMVectoritem1)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- Name and comment by locale [``[ImeIJMVectoritem1]``](#ImeIJMVectoritem1)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\- TblWznmRMTableMVector [``[ImeIRMTableMVector1]``](#ImeIRMTableMVector1)
<br>&nbsp;&nbsp;&nbsp;&nbsp;\- TblWznmRMStubMStub [``[ImeIRMStubMStub]``](#ImeIRMStubMStub)

[//]: # (IP structure - END)

Details
---

### 1 TblWznmCRelation ``[ImeICRelation]``

[//]: # (IP ImeICRelation.superUse - BEGIN)

Use:

[//]: # (IP ImeICRelation.superUse - END)

[//]: # (IP ImeICRelation.columns - BEGIN)

Column|Content|
-|-|
iref (ubigint)|ref|

[//]: # (IP ImeICRelation.columns - END)

### 2 Relation ``[ImeIMRelation]``

[//]: # (IP ImeIMRelation.superUse - BEGIN)

Use:

[//]: # (IP ImeIMRelation.superUse - END)

[//]: # (IP ImeIMRelation.columns - BEGIN)

Column|Content|
-|-|
iref (ubigint)|ref|
srefIxVBasetype (string)|type<br>grp: owning user group 1:n<br>own: owner 1:n<br>_11: 1:1<br>_1n: 1:n<br>_1npref: pref sub to 1:n<br>_1nsub1n: 1:n sub to 1:n<br>mn: m:n<br>mnsubmn: m:n sub to m:n<br>mnpref: pref sub to m:n<br>drv: univ derivate<br>drvsub: fixed sub to univ derivate<br>drvusub: univ sub to univ derivate<br>inc: inclusion<br>j: jump table 1:n<br>jpref: pref sub to jump table 1:n<br>clust: cluster 1:n<br>aux: aux 1:n<br>auxpref: pref aux to aux 1:n<br>h1n: hierarchical 1:n<br>u1n: universal 1:n<br>u1nsub: 1:n sub to universal 1:n<br>u1nsubpref: pref sub to universal 1:n<br>u1nsubinc: inclusion sub to univ 1:n<br>u1nsub11: 1:1 sub to universal 1:n<br>umn: universal m:n<br>um1n: any main table 1:n<br>a1n: attribute 1:n<br>au1n: attr universal 1:n<br>au1nsub: spec sub to attr univ 1:n<br>as1n: attr string ref 1:n<br>asmn: attr string refs m:n<br>lu1n: list fct univ 1:n<br>lu1nsub: sub to list fct univ 1:n<br>lu1nlsub: list fct sub to lu1n<br>l1nop: operator sub to l1n/lu1n<br>l1noppr: partner sub 1:n to l1nop<br>l1n: list fct 1:n<br>lmn: list fct m:n<br>lmnop: operator sub to lmn<br>lmnoppr: partner sub 1:n to lmnop|
irefRefWznmCRelation (ubigint)|TblWznmCRelation|
irefSupRefWznmMRelation (ubigint)|super relation|
srefSupIxVSubrole (string)|super relation<br>void: none<br>from1n: from table<br>to1n: to table<br>submn: T table<br>pref: preferred<br>frompref: preferred in from table<br>topref: preferred in to table<br>r1n: rel table<br>mn1n: m:n rel table<br>mod: modifier<br>sub: 1:n sub<br>subl: 1:n sub with list fct<br>subinc: inclusion sub<br>sub11: 1:1 sub<br>sub1n: S table<br>pr1: partner 1<br>pr2: partner 2<br>op: list operator<br>toum1n: to any main table<br>spec: specification|
srefFrRefWznmMTable (string)|from table|
srefFrsRefWznmMSubset (string)|from subset|
srefToRefWznmMTable (string)|to table|
srefTosRefWznmMSubset (string)|to subset|
srefRefWznmMTable (string)|table|
Prefix (string)|prefix|
srefsKOption (string)|options<br>self: self-reference<br>preffrom: preferred in from table<br>prefto: preferred in to table<br>enumfrom: enum by from table<br>enumto: enum by to table<br>pref: preferred in to table<br>enum: enumerated<br>ins: insert operation<br>rmv: remove operation<br>ina: insert after operation<br>swp: swap operation<br>affil: affiliation determining|

[//]: # (IP ImeIMRelation.columns - END)

### 2.1 Names ``[ImeIAMRelationTitle]``

[//]: # (IP ImeIAMRelationTitle.superUse - BEGIN)

Super import: relation (1:N)

Use:

[//]: # (IP ImeIAMRelationTitle.superUse - END)

[//]: # (IP ImeIAMRelationTitle.columns - BEGIN)

Column|Content|
-|-|
srefX1IxVType (string)|type<br>fromsngshort: from singular short form<br>fromsngfull: from singular full title<br>tosngshort: to singular short form<br>tosngfull: to singular full title<br>fromplshort: from plural short form<br>fromplfull: from plural full title<br>toplshort: to plural short form<br>toplfull: to plural full title|
srefX2RefWznmMLocale (string)|locale|
Title (string)|name|

[//]: # (IP ImeIAMRelationTitle.columns - END)

### 3 Stub ``[ImeIMStub]``

[//]: # (IP ImeIMStub.superUse - BEGIN)

Use:

[//]: # (IP ImeIMStub.superUse - END)

[//]: # (IP ImeIMStub.columns - BEGIN)

Column|Content|
-|-|
srefIxVBasetype (string)|type<br>tco: single table column<br>cust: custom implementation|
srefRefWznmMTable (string)|table|
srefRefWznmMSubset (string)|subset|
sref (string)|identifier|
Hierarch (bool)|hierarchical|
srefRefWznmMTablecol (string)|table column|
Localized (bool)|localized|
Example (string)|example|

[//]: # (IP ImeIMStub.columns - END)

### 4 Table ``[ImeIMTable]``

[//]: # (IP ImeIMTable.superUse - BEGIN)

Use:

[//]: # (IP ImeIMTable.superUse - END)

[//]: # (IP ImeIMTable.columns - BEGIN)

Column|Content|
-|-|
srefIxVBasetype (string)|type<br>main: main<br>aux: auxiliary<br>rel: m:n<br>jump: jump<br>clust: cluster<br>list: list<br>opr: list operator<br>sub1n: sub 1:n for 1:n<br>submn: sub 1:n for m:n<br>qry: query|
srefRefIxVTbl (string)|reference<br>void: none<br>qry: query<br>rel: relation|
irefRefUref (ubigint)|reference|
sref (string)|identifier|
Short (string)|acronym|
unqSrefsWznmMTablecol (string)|table column|
Comment (string)|comment|

[//]: # (IP ImeIMTable.columns - END)

### 4.1 Load functions ``[ImeIAMTableLoadfct]``

[//]: # (IP ImeIAMTableLoadfct.superUse - BEGIN)

Super import: table (1:N)

Use:

[//]: # (IP ImeIAMTableLoadfct.superUse - END)

[//]: # (IP ImeIAMTableLoadfct.columns - BEGIN)

Column|Content|
-|-|
srefIxVLoadtype (string)|load type<br>confirm: check presence<br>count: record count<br>ref: single ref<br>refs: set of refs<br>rec: single record<br>rst: record set<br>string: single string value<br>uint: single uint value<br>hrefsup: set of refs hier. up<br>hrefsdown: set of refs hier. down<br>hrstup: record set hier. up<br>hrstdown: record set hier. down|
Fctname (string)|function name|
ldSrefWznmMTablecol (string)|load table column|
lbySrefsWznmMTablecol (string)|table column|
ordSrefsWznmMTablecol (string)|table column|
srefIxVLimtype (string)|limitation type<br>void: none<br>first: single record<br>limofs: limit/offset parameters|

[//]: # (IP ImeIAMTableLoadfct.columns - END)

### 4.2 Names ``[ImeIAMTableTitle]``

[//]: # (IP ImeIAMTableTitle.superUse - BEGIN)

Super import: table (1:N)

Use:

[//]: # (IP ImeIAMTableTitle.superUse - END)

[//]: # (IP ImeIAMTableTitle.columns - BEGIN)

Column|Content|
-|-|
srefX1IxVType (string)|type<br>sngshort: singular short form<br>sngfull: singular full title<br>plfull: plural full title|
srefX2RefWznmMLocale (string)|locale|
srefIxWznmVGender (string)|gender<br>m: male<br>f: female<br>n: neuter|
Title (string)|name|

[//]: # (IP ImeIAMTableTitle.columns - END)

### 4.3 Feature check ``[ImeIMCheck]``

[//]: # (IP ImeIMCheck.superUse - BEGIN)

Super import: table (1:N)

Use:

[//]: # (IP ImeIMCheck.superUse - END)

[//]: # (IP ImeIMCheck.columns - BEGIN)

Column|Content|
-|-|
srefIxVBasetype (string)|type<br>eq: table column equals<br>incl: table column includes<br>leaf: leaf of hierarchical table<br>sbs: part of subsets<br>cust: custom check|
srefRefWznmMTablecol (string)|table column|
sref (string)|identifier|
Comment (string)|comment|

[//]: # (IP ImeIMCheck.columns - END)

### 4.4 Subset ``[ImeIMSubset]``

[//]: # (IP ImeIMSubset.superUse - BEGIN)

Super import: table (1:N)

Use:

[//]: # (IP ImeIMSubset.superUse - END)

[//]: # (IP ImeIMSubset.columns - BEGIN)

Column|Content|
-|-|
sref (string)|identifier|
Short (string)|acronym|
Cond (string)|condition rule|
Comment (string)|comment|

[//]: # (IP ImeIMSubset.columns - END)

### 4.4.1 Names ``[ImeIAMSubsetTitle]``

[//]: # (IP ImeIAMSubsetTitle.superUse - BEGIN)

Super import: subset (1:N)

Use:

[//]: # (IP ImeIAMSubsetTitle.superUse - END)

[//]: # (IP ImeIAMSubsetTitle.columns - BEGIN)

Column|Content|
-|-|
srefX1IxVType (string)|type<br>sngshort: singular short form<br>sngfull: singular full title<br>plfull: plural full title|
srefX2RefWznmMLocale (string)|locale|
srefIxWznmVGender (string)|gender<br>m: male<br>f: female<br>n: neuter|
Title (string)|name|

[//]: # (IP ImeIAMSubsetTitle.columns - END)

### 4.4.2 TblWznmRMSubsetMSubset ``[ImeIRMSubsetMSubset]``

[//]: # (IP ImeIRMSubsetMSubset.superUse - BEGIN)

Super import: subset (1:N)

Use:

[//]: # (IP ImeIRMSubsetMSubset.superUse - END)

[//]: # (IP ImeIRMSubsetMSubset.columns - BEGIN)

Column|Content|
-|-|
srefBsbRefWznmMSubset (string)|subset|
srefIxVReltype (string)|relation type<br>ainb: a includes b<br>bina: b includes a<br>compl: complement<br>disj: disjointedness<br>xsec: intersection|

[//]: # (IP ImeIRMSubsetMSubset.columns - END)

### 4.5 Table column ``[ImeIMTablecol]``

[//]: # (IP ImeIMTablecol.superUse - BEGIN)

Super import: table (1:N)

Use:

[//]: # (IP ImeIMTablecol.superUse - END)

[//]: # (IP ImeIMTablecol.columns - BEGIN)

Column|Content|
-|-|
srefIxVBasetype (string)|type<br>idref: identifying reference<br>idsref: identidying string reference<br>klref: key list reference<br>tblref: table reference<br>tblsref: table string reference<br>vecref: vector reference<br>uvsref: universal vector string reference<br>grp: owning user group reference<br>own: owner reference<br>enum: enumerator<br>lvl: level in hierarchy<br>intval: integer value<br>dblval: double value<br>boolval: boolean value<br>txtval: text value<br>timeval: time value<br>expr: code expression|
srefRefWznmMSubset (string)|subset|
irefRefWznmMRelation (ubigint)|relation|
srefFctIxVTbl (string)|functionality<br>void: none<br>tbl: table<br>vec: vector|
srefFctUref (string)|functionality|
sref (string)|identifier|
Short (string)|acronym|
srefIxVSubtype (string)|subtype<br>void: none<br>klrefopt: optional<br>klrefsng: single<br>klrefmult: multi<br>trefspec: specific table<br>trefuniv: universal table<br>trefmin: minor reference<br>trefclu: cluster table<br>tsrefsng: single<br>tsrefmult: multi<br>vreflin: linear vector index<br>vrefand: AND mask for mc vector<br>enauto: automatic increment<br>enspec: specific numbering<br>tinyint: integer / byte (8bit)<br>utinyint: unsigned integer / byte (8bit)<br>smallint: integer (16bit)<br>usmallint: unsigned integer (16bit)<br>int: integer (32bit)<br>uint: unsigned integer (32bit)<br>bigint: integer (64bit)<br>ubigint: unsigned integer (64bit)<br>txt5: max. 5 characters<br>txt10: max. 10 characters<br>txt30: max. 30 characters<br>txt50: max. 50 characters<br>txt100: max. 100 characters<br>txt255: max. 255 characters<br>txtlong: text field (unlimited)<br>txtbase64: Base64 encoded binary (unlimited)<br>tmdate: date<br>tmtime: time<br>tmstamp: time stamp<br>tmustamp: time stamp with usecs|
srefIxVAxisfct (string)|axis functionality<br>void: none<br>pt: point<br>spt: starting point<br>ept: end point|
srefsKOption (string)|options<br>idx: indexed|
Principal (bool)|principal|
Eponymous (bool)|eponymous for record|

[//]: # (IP ImeIMTablecol.columns - END)

### 4.5.1 Names ``[ImeIAMTablecolTitle]``

[//]: # (IP ImeIAMTablecolTitle.superUse - BEGIN)

Super import: table column (1:N)

Use:

[//]: # (IP ImeIAMTablecolTitle.superUse - END)

[//]: # (IP ImeIAMTablecolTitle.columns - BEGIN)

Column|Content|
-|-|
srefX1IxVType (string)|type<br>short: short form<br>full: full title|
srefX2RefWznmMLocale (string)|locale|
Title (string)|name|

[//]: # (IP ImeIAMTablecolTitle.columns - END)

### 4.6 Vector ``[ImeIMVector2]``

[//]: # (IP ImeIMVector2.superUse - BEGIN)

Super import: table (1:N)

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

### 4.6.1 Names ``[ImeIAMVectorTitle2]``

[//]: # (IP ImeIAMVectorTitle2.superUse - BEGIN)

Super import: vector (1:N)

Use:

[//]: # (IP ImeIAMVectorTitle2.superUse - END)

[//]: # (IP ImeIAMVectorTitle2.columns - BEGIN)

Column|Content|
-|-|
srefX1IxVType (string)|type<br>short: short form<br>full: full title|
srefX2RefWznmMLocale (string)|locale|
Title (string)|name|

[//]: # (IP ImeIAMVectorTitle2.columns - END)

### 4.6.2 Vector item ``[ImeIMVectoritem2]``

[//]: # (IP ImeIMVectoritem2.superUse - BEGIN)

Super import: vector (1:N)

Use:

[//]: # (IP ImeIMVectoritem2.superUse - END)

[//]: # (IP ImeIMVectoritem2.columns - BEGIN)

Column|Content|
-|-|
sref (string)|identifier|
Avail (string)|availability rule|
Implied (string)|rule for implied|

[//]: # (IP ImeIMVectoritem2.columns - END)

### 4.6.2.1 Name and comment by locale ``[ImeIJMVectoritem2]``

[//]: # (IP ImeIJMVectoritem2.superUse - BEGIN)

Super import: vector item (1:N)

Use:

[//]: # (IP ImeIJMVectoritem2.superUse - END)

[//]: # (IP ImeIJMVectoritem2.columns - BEGIN)

Column|Content|
-|-|
srefX1RefWznmMLocale (string)|locale|
Title (string)|Title|
Comment (string)|Comment|

[//]: # (IP ImeIJMVectoritem2.columns - END)

### 4.6.3 TblWznmRMTableMVector ``[ImeIRMTableMVector2]``

[//]: # (IP ImeIRMTableMVector2.superUse - BEGIN)

Super import: vector (1:N)

Use:

[//]: # (IP ImeIRMTableMVector2.superUse - END)

[//]: # (IP ImeIRMTableMVector2.columns - BEGIN)

Column|Content|
-|-|
srefRefWznmMTable (string)|table|
srefRefWznmMSubset (string)|subset|

[//]: # (IP ImeIRMTableMVector2.columns - END)

### 5 Vector ``[ImeIMVector1]``

[//]: # (IP ImeIMVector1.superUse - BEGIN)

Use:

[//]: # (IP ImeIMVector1.superUse - END)

[//]: # (IP ImeIMVector1.columns - BEGIN)

Column|Content|
-|-|
srefIxVBasetype (string)|type<br>lin: linear<br>or: multiple-choice<br>klst: key list<br>vlst: value list|
sref (string)|identifier|
osrefWznmKTaggrp (string)|source tag group<br>access: VecXxxxWAccess item<br>adrtype: address type<br>ctdet: contact detail<br>ctry: country<br>expstate: VecXxxxVExpstate item<br>iop: VecXxxxVIop item<br>lat: VecXxxxVLat item<br>lop: VecXxxxVLop item<br>mimetype: MIME type<br>no: no thing<br>none: none<br>oolop: VecXxxxVOolop item<br>prs: default person<br>prstit: person title<br>qrystate: VecXxxxVQrystate item<br>recaccess: VecXxxxVRecaccess item<br>reqitmode: VecXxxxVReqitmode item<br>sex: sex<br>start: login card<br>stdalr: standard alert message<br>stdrel: standard relation title<br>stdtbl: standard table title<br>stdtco: standard table column title<br>stdvec: standard vector title<br>uiaccess: VecXxxxWUiaccess item<br>userlevel: VecXxxxVUserlevel item<br>usrste: user state<br>wkday: weekday|
srefsKOption (string)|options<br>noloc: non-localized<br>notit: no titles<br>cmt: comments<br>apdfed: append to feed<br>filfed: fill feed|

[//]: # (IP ImeIMVector1.columns - END)

### 5.1 Names ``[ImeIAMVectorTitle1]``

[//]: # (IP ImeIAMVectorTitle1.superUse - BEGIN)

Super import: vector (1:N)

Use:

[//]: # (IP ImeIAMVectorTitle1.superUse - END)

[//]: # (IP ImeIAMVectorTitle1.columns - BEGIN)

Column|Content|
-|-|
srefX1IxVType (string)|type<br>short: short form<br>full: full title|
srefX2RefWznmMLocale (string)|locale|
Title (string)|name|

[//]: # (IP ImeIAMVectorTitle1.columns - END)

### 5.2 Vector item ``[ImeIMVectoritem1]``

[//]: # (IP ImeIMVectoritem1.superUse - BEGIN)

Super import: vector (1:N)

Use:

[//]: # (IP ImeIMVectoritem1.superUse - END)

[//]: # (IP ImeIMVectoritem1.columns - BEGIN)

Column|Content|
-|-|
sref (string)|identifier|
Avail (string)|availability rule|
Implied (string)|rule for implied|

[//]: # (IP ImeIMVectoritem1.columns - END)

### 5.2.1 Name and comment by locale ``[ImeIJMVectoritem1]``

[//]: # (IP ImeIJMVectoritem1.superUse - BEGIN)

Super import: vector item (1:N)

Use:

[//]: # (IP ImeIJMVectoritem1.superUse - END)

[//]: # (IP ImeIJMVectoritem1.columns - BEGIN)

Column|Content|
-|-|
srefX1RefWznmMLocale (string)|locale|
Title (string)|Title|
Comment (string)|Comment|

[//]: # (IP ImeIJMVectoritem1.columns - END)

### 5.3 TblWznmRMTableMVector ``[ImeIRMTableMVector1]``

[//]: # (IP ImeIRMTableMVector1.superUse - BEGIN)

Super import: vector (1:N)

Use:

[//]: # (IP ImeIRMTableMVector1.superUse - END)

[//]: # (IP ImeIRMTableMVector1.columns - BEGIN)

Column|Content|
-|-|
srefRefWznmMTable (string)|table|
srefRefWznmMSubset (string)|subset|

[//]: # (IP ImeIRMTableMVector1.columns - END)

### 6 TblWznmRMStubMStub ``[ImeIRMStubMStub]``

[//]: # (IP ImeIRMStubMStub.superUse - BEGIN)

Use:

[//]: # (IP ImeIRMStubMStub.superUse - END)

[//]: # (IP ImeIRMStubMStub.columns - BEGIN)

Column|Content|
-|-|
srefSupRefWznmMStub (string)|stub|
srefSubRefWznmMStub (string)|stub|

[//]: # (IP ImeIRMStubMStub.columns - END)

<em>Markdown for WhizniumSBE 0.9.12 auto-generated (what else ;-) ) by WhizniumSBE on 16 Sep 2018</em>
