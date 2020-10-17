# mms

mms.pdu_type.id

Attribute | Value
--- | ---
**IE Name** | .id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

mms.pdu_type.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

mms.req.invoke_id
mms.req.confirm_svc.id

Attribute | Value
--- | ---
**IE Name** | .id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

mms.req.confirm_svc.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

mms.req.listOfModifier    SEQUENCE OF Modifier OPTIONAL,
mms.req.CS-Request-Detail    OPTIONAL


mms.uncnf.unconfirm_svc.id

Attribute | Value
--- | ---
**IE Name** | .id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

mms.uncnf.unconfirm_svc.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

mms.uncnf.CS-Request-Detail    OPTIONAL


mms.resp.invoke_id
mms.resp.confirm_svc.id

Attribute | Value
--- | ---
**IE Name** | .id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

mms.resp.confirm_svc.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

mms.resp.CS-Request-Detail    OPTIONAL

mms.error.invoke_id
mms.error.modifierPosition [1] IMPLICIT Unsigned32 OPTIONAL,
mms.error.serviceError  [2] IMPLICIT ServiceError

text
CS-Request-Detail ::= CHOICE {
				-- see ISO 9506-2
				}


--********************************** COMMON MMS TYPES ***********************************

FileName ::= SEQUENCE OF GraphicString

TimeOfDay ::= OCTET STRING -- (SIZE (4 | 6))

Identifier ::= VisibleString

Integer8   ::= INTEGER
Integer16  ::= INTEGER
Integer32  ::= INTEGER


Unsigned8  ::= INTEGER
Unsigned16 ::= INTEGER
Unsigned32 ::= INTEGER


ObjectName ::= CHOICE 
	{
	vmd-specific		[0] IMPLICIT Identifier,
	domain-specific	        [1] IMPLICIT SEQUENCE
		{
		domainId 	Identifier,
		itemId		Identifier
		},
	aa-specific		[2] IMPLICIT Identifier
	}


ApplicationReference ::= SEQUENCE
	{
	ap-title		[0] ISO-8650-ACSE-1.AP-title 	        OPTIONAL,
	ap-invocation-id	[1] ISO-8650-ACSE-1.AP-invocation-identifier OPTIONAL,
	ae-qualifier		[2] ISO-8650-ACSE-1.AE-qualifier	        OPTIONAL,
	ae-invocation-id	[3] ISO-8650-ACSE-1.AE-invocation-identifier OPTIONAL
	}


Priority ::= Unsigned8

normalPriority Priority ::= 64


-- ************************************ GENERAL *************************************

Initiate-ErrorPDU ::= ServiceError

Initiate-RequestPDU ::= SEQUENCE
	{
	localDetailCalling	        	[0] IMPLICIT Integer32 OPTIONAL,
	proposedMaxServOutstandingCalling	[1] IMPLICIT Integer16,
	proposedMaxServOutstandingCalled	[2] IMPLICIT Integer16,
	proposedDataStructureNestingLevel	[3] IMPLICIT Integer8 OPTIONAL,
	mmsInitRequestDetail			[4] IMPLICIT InitRequestDetail
	}

InitRequestDetail ::= SEQUENCE
	{
	proposedVersionNumber			[0] IMPLICIT Integer16,
	proposedParameterCBB			[1] IMPLICIT ParameterSupportOptions,
	servicesSupportedCalling		[2] IMPLICIT ServiceSupportOptions
	}

Initiate-ResponsePDU ::= SEQUENCE
	{
	localDetailCalled			[0] IMPLICIT Integer32 OPTIONAL,
	negociatedMaxServOutstandingCalling	[1] IMPLICIT Integer16,
	negociatedMaxServOutstandingCalled	[2] IMPLICIT Integer16,
	negociatedDataStructureNestingLevel	[3] IMPLICIT Integer8 OPTIONAL,
	mmsInitResponseDetail			[4] IMPLICIT InitResponseDetail
	}

InitResponseDetail ::= SEQUENCE
	{
	negociatedVersionNumber			[0] IMPLICIT Integer16,
	negociatedParameterCBB			[1] IMPLICIT ParameterSupportOptions,
	servicesSupportedCalled			[2] IMPLICIT ServiceSupportOptions
	}


ParameterSupportOptions ::= BIT STRING {
	str1 (0),
	str2 (1),
	vnam (2),
	valt (3),
	vadr (4),
	vsca (5),
	tpy  (6),
	vlis (7),
	real (8),
	cei  (10)
	}


ServiceSupportOptions ::= BIT STRING 
	{
	status					(0),	
	getNameList				(1), 	
	identify				(2), 		
	rename					(3),	
	read					(4),	
	write					(5),	
	getVariableAccessAttributes		(6),	
	defineNamedVariable			(7),	
	defineScatteredAccess			(8),	
	getScatteredAccessAttributes		(9),	
	deleteVariableAccess			(10),		
	defineNamedVariableList			(11),	
	getNamedVariableListAttributes		(12),	
	deleteNamedVariableList			(13),	
	defineNamedType				(14),		
	getNamedTypeAttributes			(15),	
	deleteNamedType				(16),	
	input					(17),	
	output					(18),	
	takeControl				(19),	
	relinquishControl			(20),	
	defineSemaphore				(21),	
	deleteSemaphore				(22),	
	reportSemaphoreStatus			(23),	
	reportPoolSemaphoreStatus		(24),	
	reportSemaphoreEntryStatus		(25),	
	initiateDownloadSequence		(26),	
	downloadSegment				(27),	
	terminateDownloadSequence		(28),	
	initiateUploadSequence			(29),	
	uploadSegment				(30),	
	terminateUploadSequence			(31),	
	requestDomainDownload			(32),	
	requestDomainUpload			(33),	
	loadDomainContent			(34),	
	storeDomainContent			(35),	
	deleteDomain				(36),	
	getDomainAttributes			(37),	
	createProgramInvocation			(38),	
	deleteProgramInvocation			(39),	
	start					(40),	
	stop					(41),	
	resume					(42),	
	reset					(43),	
	kill					(44),	
	getProgramInvocationAttributes		(45),	
	obtainFile				(46),	
	defineEventCondition			(47),	
	deleteEventCondition			(48),	
	getEventConditionAttributes		(49),	
	reportEventConditionStatus		(50),	
	alterEventConditionMonitoring		(51),	
	triggerEvent				(52),	
	defineEventAction			(53),	
	deleteEventAction			(54),	
	getEventActionAttributes		(55),	
	reportActionStatus			(56),	
	defineEventEnrollment			(57),	
	deleteEventEnrollment			(58),	
	alterEventEnrollment			(59),	
	reportEventEnrollmentStatus		(60),	
	getEventEnrollmentAttributes		(61),	
	acknowledgeEventNotification		(62),	
	getAlarmSummary				(63),	
	getAlarmEnrollmentSummary		(64),	
	readJournal				(65),	
	writeJournal				(66),	
	initializeJournal			(67),	
	reportJournalStatus			(68),	
	createJournal				(69),	
	deleteJournal				(70),	
	getCapabilityList			(71),	
	fileOpen				(72),	
	fileRead				(73),	
	fileClose				(74),	
	fileRename				(75),	
	fileDelete				(76),	
	fileDirectory				(77),	
	unsolicitedStatus			(78),
	informationReport			(79),
	eventNotification			(80),
	attachToEventCondition			(81),
	attachToSemaphore			(82),
	conclude				(83),
	cancel					(84)
	}

---------------------------------- CONCLUDE --------------------------------

Conclude-RequestPDU ::= NULL

Conclude-ResponsePDU ::= NULL

Conclude-ErrorPDU ::= ServiceError

---------------------------------- CANCEL --------------------------------

Cancel-RequestPDU ::= Unsigned32	-- originalInvokeID

Cancel-ResponsePDU ::= Unsigned32 	-- originalInvokeID

Cancel-ErrorPDU ::= SEQUENCE
	{
	originalInvokeID	[0] IMPLICIT Unsigned32,
	serviceError		[1] IMPLICIT ServiceError
	}

------------------------------ Service-Error --------------------------------

ServiceError ::= SEQUENCE 
	{	
	errorClass	[0] CHOICE
		{ 
		vmd-state 	[0] IMPLICIT INTEGER  	
			{	
			other 					(0),			       
			vmd-state-conflict 			(1),		
			vmd-operational-problem 		(2), 
			domain-transfer-problem 		(3),	
			state-machine-id-invalid 		(4)	
                  	},
		application-reference 	[1] IMPLICIT INTEGER
		       	{
			other 					(0),
			aplication-unreachable 			(1),
			connection-lost 			(2),
			application-reference-invalid 		(3),
			context-unsupported 			(4)
			},
		definition 			[2] IMPLICIT INTEGER
			{
			other 					(0),
			object-undefined 			(1),
			invalid-address 			(2),
			type-unsupported 			(3),
			type-inconsistent 			(4),
			object-exists 				(5),
			object-attribute-inconsistent  	        (6)
			},
		resource 			[3] IMPLICIT INTEGER
			{
			other 					(0),
			memory-unavailable			(1),
			processor-resource-unavailable		(2),
			mass-storage-unavailable		(3),
			capability-unavailable			(4),
			capability-unknown			(5)
		       	},
		service 			[4] IMPLICIT INTEGER
			{	
			other 					(0),
			primitives-out-of-sequence		(1),
			object-sate-conflict			(2),
			pdu-size				(3),
			continuation-invalid			(4),
			object-constraint-conflict		(5)
		      	},
		service-preempt 		[5] IMPLICIT INTEGER
		      	{	
			other					(0),
			timeout					(1),
			deadlock				(2),
			cancel					(3)
		      	},
		time-resolution 		[6] IMPLICIT INTEGER
		      	{	
			other					(0),
			unsupportable-time-resolution 		(1)
		      	},
		access	 			[7] IMPLICIT INTEGER
		      	{
			other					(0),
			object-access-unsupported		(1),
			object-non-existent			(2),
			object-access-denied			(3),
			object-invalidated			(4)
		 	},
		initiate 			[8] IMPLICIT INTEGER
		     	{
			other					(0),
			version-incompatible			(1),
			max-segment-insufficient		(2),
			max-services-outstanding-calling-insufficient (3),
			max-services-outstanding-called-insufficient  (4),
			service-CBB-insufficient		(5),
			parameter-CBB-insufficient		(6),
			nesting-level-insufficient		(7)
			},
		conclude 			[9] IMPLICIT INTEGER
		     	{
			other					(0),
			further-communication-required 		(1)
			},
		cancel 				[10] IMPLICIT INTEGER
		     	{
			other					(0),
			invoke-id-unknown			(1),
			cancel-not-possible			(2)
			},
		file 				[11] IMPLICIT INTEGER
		     	{
			other					(0),
			filename-ambiguous			(1),
			file-busy				(2),
			filename-syntax-error			(3),
			content-type-invalid			(4),
			position-invalid			(5),
			file-acces-denied			(6),
			file-non-existent			(7),
			duplicate-filename			(8),
			insufficient-space-in-filestore		(9)
			},
		others	 		        [12] IMPLICIT INTEGER
	        },
	additionalCode			[1] IMPLICIT INTEGER OPTIONAL,
	additionalDescription 		[2] IMPLICIT VisibleString OPTIONAL,
	serviceSpecificInformation	[3] CHOICE
			{
			obtainFile			[0] IMPLICIT ObtainFile-Error,
			start				[1] IMPLICIT Start-Error,
			stop				[2] IMPLICIT Stop-Error,
			resume				[3] IMPLICIT Resume-Error,
			reset				[4] IMPLICIT Reset-Error,
			deleteVariableAccess		[5] IMPLICIT DeleteVariableAccess-Error,
			deleteNamedVariableList		[6] IMPLICIT DeleteNamedVariableList-Error,
			deleteNamedType			[7] IMPLICIT DeleteNamedType-Error,
			defineEventEnrollment-Error	[8] DefineEventEnrollment-Error,
			fileRename			[9] IMPLICIT FileRename-Error,
			additionalService		[10] AdditionalServiceError
			} OPTIONAL
	}


---------------------------------- REJECT --------------------------------

RejectPDU ::= SEQUENCE
	{
	originalInvokeID		[0] IMPLICIT Unsigned32 OPTIONAL,
	rejectReason 			    CHOICE 
		{
		confirmed-requestPDU		[1] IMPLICIT INTEGER 
			{
			other					(0),
			unrecognized-service			(1),
			unrecognized-modifier			(2),
			invalid-invokeID			(3),
			invalid-argument			(4),
			invalid-modifier			(5),
			max-serv-outstanding-exceeded		(6),
			max-recursion-exceeded			(8),
			value-out-of-range			(9)
			},

		confirmed-responsePDU		[2] IMPLICIT INTEGER 
			{
			other					(0),
			unrecognized-service			(1),
			invalid-invokeID			(2),
			invalid-result				(3),
			max-recursion-exceeded			(5),
			value-out-of-range			(6) 	
			},	
		
		confirmed-errorPDU		[3] IMPLICIT INTEGER 
			{
			other					(0),
			unrecognized-service			(1),
			invalid-invokeID			(2),
			invalid-serviceError			(3),
			value-out-of-range			(4) 	 
			} ,			
			
		unconfirmedPDU			[4] IMPLICIT INTEGER
			{
			other					(0),
			unrecognized-service			(1),
			invalid-argument			(2),
			max-recursion-exceeded			(3),
			value-out-of-range			(4) 	
			},

		pdu-error			[5] IMPLICIT INTEGER
			{
			unknown-pdu-type			(0),
			invalid-pdu				(1),
			illegal-acse-mapping			(2)
			},

		cancel-requestPDU		[6] IMPLICIT INTEGER
			{
			other					(0),
			invalid-invokeID			(1)	
			},	

		cancel-responsePDU	        [7] IMPLICIT INTEGER
			{
			other					(0),
			invalid-invokeID			(1)	
			},

		cancel-errorPDU			[8] IMPLICIT INTEGER
			{
			other					(0),
			invalid-invokeID			(1),
			invalid-serviceError			(2),
			value-out-of-range			(3) 	
			},

		conclude-requestPDU		[9] IMPLICIT INTEGER
			{
			other					(0),
			invalid-argument			(1)	
			},	

		conclude-responsePDU	        [10] IMPLICIT INTEGER
			{
			other					(0),
			invalid-result				(1)	
			},

		conclude-errorPDU		[11] IMPLICIT INTEGER
			{
			other					(0),
			invalid-serviceError			(1),
			value-out-of-range			(2) 	
			}
		}
	}


-- *************************************** VMD ********************************************


Status-Request ::= BOOLEAN

Status-Response ::= SEQUENCE {
    vmdLogicalStatus	     [0] IMPLICIT INTEGER {
      state-changes-allowed	  (0),
      no-state-changes-allowed	  (1),
      limited-services-allowed	  (2),
      support-services-allowed	  (3)
      },
    vmdPhysicalStatus	     [1] IMPLICIT INTEGER {
      operational		  (0),
      partially-operational	  (1),
      inoperable		  (2),
      needs-commissioning	  (3)
      },
    localDetail		     [2] IMPLICIT BIT STRING(SIZE(0..128)) OPTIONAL

    }

------------------------------- UNSOLICITEDSTATUS --------------------------------

UnsolicitedStatus ::= Status-Response

--------------------------------- GETNAMELIST --------------------------------

GetNameList-Request ::= SEQUENCE
	{
	extendedObjectClass [0] CHOICE
		{
		objectClass		[0] IMPLICIT INTEGER
			{
			nammedVariable		(0),
			scatteredAccess		(1),
			namedVariableList	(2),
			namedType		(3),
			semaphore		(4),
			eventCondition		(5),
			eventAction		(6),
			eventEnrollment		(7),
			journal			(8),
			domain			(9),
			programInvocation	(10),
			operatorStation		(11)
			}
		},
	objectScope 		[1] CHOICE
		{
		vmdSpecific		[0] IMPLICIT NULL,
		domainSpecific		[1] IMPLICIT Identifier,
		aaSpecific		[2] IMPLICIT NULL
		},
	continueAfter 	[2] IMPLICIT Identifier OPTIONAL
	}

GetNameList-Response ::= SEQUENCE
	{
	listOfIdentifier	[0] IMPLICIT SEQUENCE OF Identifier,
	moreFollows		[1] IMPLICIT BOOLEAN DEFAULT TRUE
	}


---------------------------------- IDENTIFY --------------------------------

Identify-Request ::= NULL

Identify-Response ::= SEQUENCE {
	vendorName		[0] IMPLICIT VisibleString,
	modelName		[1] IMPLICIT VisibleString,
	revision		[2] IMPLICIT VisibleString,
	listOfAbstractSyntaxes	[3] IMPLICIT SEQUENCE OF OBJECT IDENTIFIER OPTIONAL
	}

---------------------------------- RENAME --------------------------------

Rename-Request ::= SEQUENCE 
	{
	extendedObjectClass	[0] CHOICE {
	objectClass			[0] IMPLICIT INTEGER
		{
		namedVariable		(0),
		scatteredAccess		(1),
		namedVariableList	(2),
		namedType		(3),
		semaphore		(4),
		eventCondition		(5),
		eventAction		(6),
		eventEnrollment		(7),
		journal			(8),
		domain			(9),
		programInvocation	(10),
		operatorStation		(11)
		}

	    },
	currentName 		[1] ObjectName,
	newIdentifier		[2] IMPLICIT Identifier
      	}

Rename-Response ::= NULL

---------------------------------- GET CAPABILITY LIST --------------------------------

GetCapabilityList-Request ::= SEQUENCE {
	continueAfter	VisibleString OPTIONAL
	}

GetCapabilityList-Response ::= SEQUENCE {
	listOfCapabilities	[0] IMPLICIT SEQUENCE OF VisibleString,
	moreFollows		[1] IMPLICIT BOOLEAN DEFAULT TRUE
	}





-- ************************************* DOMAIN ****************************************

InitiateDownloadSequence-Request ::= SEQUENCE
	{
	domainName		[0] IMPLICIT Identifier,
	listOfCapabilities	[1] IMPLICIT SEQUENCE OF VisibleString,
	sharable		[2] IMPLICIT BOOLEAN
	}

InitiateDownloadSequence-Response ::= NULL

---------------------------------- DOWNLOAD SEGMENT -----------------------------------

DownloadSegment-Request ::= Identifier

DownloadSegment-Response ::= SEQUENCE
	{
	loadData	CHOICE {
	   non-coded		[0] IMPLICIT OCTET STRING,
	   coded		EXTERNAL
	   },
	moreFollows	[1] IMPLICIT BOOLEAN DEFAULT TRUE
	}

-------------------------------- TERMINATE DOWNLOAD -----------------------------------

TerminateDownloadSequence-Request ::= SEQUENCE
	{
	domainName	[0] IMPLICIT Identifier,
	discard		[1] IMPLICIT ServiceError OPTIONAL
	}
	
TerminateDownloadSequence-Response ::= NULL 

-------------------------------- INITIATE UPLOAD -----------------------------------

InitiateUploadSequence-Request ::= Identifier 	-- Domain Name

InitiateUploadSequence-Response ::= SEQUENCE
	{
	ulsmID			[0] IMPLICIT Integer32,
	listOfCapabilities	[1] IMPLICIT SEQUENCE OF VisibleString
	}

---------------------------------- UPLOAD SEGMENT -----------------------------------

UploadSegment-Request ::= Integer32	-- ULSM Identifier

UploadSegment-Response ::= SEQUENCE
	{
	loadData	CHOICE {
	   non-coded		[0] IMPLICIT OCTET STRING,
	   coded		EXTERNAL
	   },
	moreFollows	[1] IMPLICIT BOOLEAN DEFAULT TRUE
	}

-------------------------------- TERMINATE UPLOAD -----------------------------------

TerminateUploadSequence-Request ::= Integer32	-- ULSM Identifer

TerminateUploadSequence-Response ::= NULL

----------------------------- REQUEST DOMAIN DOWNLOAD -----------------------------------

RequestDomainDownload-Request ::= SEQUENCE
	{
	domainName		[0] IMPLICIT Identifier,
	listOfCapabilities	[1] IMPLICIT SEQUENCE OF VisibleString OPTIONAL,
	sharable		[2] IMPLICIT BOOLEAN,
	fileName		[4] IMPLICIT FileName
	}
RequestDomainDownload-Response ::= NULL

----------------------------- REQUEST DOMAIN UPLOAD -----------------------------------

RequestDomainUpload-Request ::= SEQUENCE
	{
	domainName	[0] IMPLICIT Identifier,
	fileName	[1] IMPLICIT FileName
	}

RequestDomainUpload-Response ::= NULL

----------------------------- LOAD DOMAIN CONTENT -----------------------------------

LoadDomainContent-Request ::= SEQUENCE
	{
	domainName		[0] IMPLICIT Identifier,
	listOfCapabilities	[1] IMPLICIT SEQUENCE OF VisibleString OPTIONAL,
	sharable		[2] IMPLICIT BOOLEAN,
	fileName		[4] IMPLICIT FileName,
	thirdParty		[5] IMPLICIT ApplicationReference OPTIONAL
	}

LoadDomainContent-Response ::= NULL

----------------------------- STORE DOMAIN CONTENT -----------------------------------

StoreDomainContent-Request ::= SEQUENCE
	{
	domainName 	[0] IMPLICIT Identifier,
	filenName	[1] IMPLICIT FileName,
	thirdParty	[2] IMPLICIT ApplicationReference OPTIONAL
	}

StoreDomainContent-Response ::= NULL

----------------------------- DELETE DOMAIN  -----------------------------------

DeleteDomain-Request ::= Identifier	-- Domain Name 

DeleteDomain-Response ::= NULL

----------------------------- GET DOMAIN ATTRIBUTES  -----------------------------------

GetDomainAttributes-Request ::= Identifier	-- Domain Name

GetDomainAttributes-Response ::= SEQUENCE
	{
	listOfCapabilities		[0] IMPLICIT SEQUENCE OF VisibleString,
	state				[1] IMPLICIT DomainState,
	mmsDeletable			[2] IMPLICIT BOOLEAN,
	sharable			[3] IMPLICIT BOOLEAN,
	listOfProgramInvocations	[4] IMPLICIT SEQUENCE OF Identifier, 	-- PI Names
	uploadInProgress		[5] IMPLICIT Integer8
	}


DomainState ::= INTEGER
	{
	non-existent	(0),
	loading		(1),
	ready		(2),
	in-use		(3),
	complete	(4),
	incomplete	(5),
	d1		(7),
	d2		(8),
	d3		(9),
	d4		(10),
	d5		(11),
	d6		(12),
	d7		(13),
	d8		(14),
	d9		(15)
	}

-- ********************************* PROGRAM INVOCATION *********************************


----------------------CREATE PROGRAM INVOCATION ---------------------

CreateProgramInvocation-Request ::= SEQUENCE
	{
	programInvocationName 	[0] IMPLICIT Identifier,
	listOfDomainName		[1] IMPLICIT SEQUENCE OF Identifier,
	reusable			[2] IMPLICIT BOOLEAN DEFAULT TRUE,
	monitorType			[3] IMPLICIT BOOLEAN OPTIONAL
		-- TRUE indicates PERMANENT monitoring
		-- FALSE indicates CURRENT monitoring
	}

CreateProgramInvocation-Response ::= NULL

----------------------DELETE PROGRAM INVOCATION ---------------------

DeleteProgramInvocation-Request   ::= Identifier	-- Program Invocation Name

DeleteProgramInvocation-Response ::= NULL

----------------------------- START ------------------------------------

Start-Request ::= SEQUENCE	
	{
	programInvocationName 	[0] IMPLICIT Identifier,
	executionArgument	CHOICE {
	    simpleString	  [1] IMPLICIT VisibleString,
	    encodedString	  EXTERNAL
	    } OPTIONAL
	}

Start-Response ::= NULL

Start-Error ::= ProgramInvocationState

----------------------------- STOP ------------------------------------

Stop-Request ::= SEQUENCE 
	{
	programInvocationName	[0] IMPLICIT Identifier
	}

Stop-Response ::= NULL

Stop-Error ::= ProgramInvocationState

---------------------------- RESUME ------------------------------------

Resume-Request ::= SEQUENCE
	{
	programInvocationName 	[0] IMPLICIT Identifier,
	executionArgument	CHOICE {
	    simpleString	  [1] IMPLICIT VisibleString,
	    encodedString	  EXTERNAL
	    } OPTIONAL
	}

Resume-Response ::= NULL

Resume-Error ::= ProgramInvocationState

------------------------------ RESET ------------------------------------

Reset-Request ::= SEQUENCE 
	{
	programInvocationName	[0] IMPLICIT Identifier
	}

Reset-Response ::= NULL

Reset-Error ::= ProgramInvocationState

------------------------------ KILL ------------------------------------

Kill-Request ::= SEQUENCE
	{
	programInvocationName	[0] IMPLICIT Identifier
	}

Kill-Response ::= NULL

--------------------------- GET PI ATTRIBUTES ------------------------------------

GetProgramInvocationAttributes-Request ::= Identifier	-- Program Invocation Name

GetProgramInvocationAttributes-Response ::= SEQUENCE
	{
	state			[0] IMPLICIT ProgramInvocationState,
	listOfDomainNames	[1] IMPLICIT SEQUENCE OF Identifier,				
	mmsDeletable		[2] IMPLICIT BOOLEAN,
	reusable		[3] IMPLICIT BOOLEAN,
	monitor			[4] IMPLICIT BOOLEAN,
	startArgument		[5] IMPLICIT VisibleString,
	executionArgument	CHOICE {
	    simpleString	  [1] IMPLICIT VisibleString,
	    encodedString	  EXTERNAL
	    } OPTIONAL
	}


ProgramInvocationState ::= INTEGER
	{
	non-existent		(0),
	unrunable		(1),
	idle			(2),
	running			(3),
	stopped			(4),
	starting		(5),
	stopping		(6),
	resuming		(7),
	resetting		(8)
	}
	-- Companion Standard may add additional values


-- *********************************** VARIABLES ****************************************


TypeSpecification ::= CHOICE 
	{
	typeName		[0] ObjectName,
	array			[1] IMPLICIT SEQUENCE
		{
		packed			[0] IMPLICIT BOOLEAN DEFAULT FALSE,
		numberOfElements	[1] IMPLICIT Unsigned32,
		elementType		[2] TypeSpecification,
		},
	structure		[2] IMPLICIT SEQUENCE
		{
		packed			[0] IMPLICIT BOOLEAN DEFAULT FALSE,
		components		[1] IMPLICIT SEQUENCE OF SEQUENCE
			{
			componentName		[0] IMPLICIT Identifier OPTIONAL,
			componentType		[1] TypeSpecification
			}
		},
	
	-- Simple Type -------- Size ---------
	boolean			[3] IMPLICIT NULL,
	bit-string		[4] IMPLICIT Integer32,
	integer			[5] IMPLICIT Unsigned8,
	unsigned		[6] IMPLICIT Unsigned8,
	octet-string		[9] IMPLICIT Integer32,
	visible-string		[10] IMPLICIT Integer32,
	generalized-time	[11] IMPLICIT NULL,
	binary-time		[12] IMPLICIT BOOLEAN,
	bcd			[13] IMPLICIT Unsigned8,
	objId			[15] IMPLICIT NULL
	}

AlternateAccess ::= SEQUENCE OF CHOICE
	{
	unnamed	AlternateAccessSelection,
	named		[5] IMPLICIT SEQUENCE 
		{
		componentName	[0] IMPLICIT Identifier,
		accesst		AlternateAccessSelection
		}
	}

AlternateAccessSelection ::= CHOICE
	{
	selectAccess	CHOICE
		{
		component	[1] IMPLICIT Identifier,
		index		[2] IMPLICIT Unsigned32,
		indexRange	[3] IMPLICIT SEQUENCE
			{
			lowIndex			[0] IMPLICIT Unsigned32,
			numberOfElements		[1] IMPLICIT Unsigned32
			},
		allElements	[4] IMPLICIT NULL	-- all array elements
		}
	}


-------------------------------- READ -------------------------------

Read-Request ::= SEQUENCE
	{
	specificationWithResult		[0] IMPLICIT BOOLEAN DEFAULT FALSE,
	variableAccessSpecificatn	[1] VariableAccessSpecification
	}


Read-Response ::= SEQUENCE
	{
	variableAccessSpecificatn [0] VariableAccessSpecification OPTIONAL,
	listOfAccessResult	  [1] IMPLICIT SEQUENCE OF AccessResult
	}

-------------------------------- WRITE -------------------------------



Write-Request ::= SEQUENCE
	{
	variableAccessSpecificatn 	VariableAccessSpecification,
	listOfData			[0] IMPLICIT SEQUENCE OF Data
	}

Write-Response ::= SEQUENCE OF CHOICE
	{
	failure		[0] IMPLICIT DataAccessError,
	success		[1] IMPLICIT NULL
	}

---------------------------- INFORMATION REPORT --------------------------------

InformationReport ::= SEQUENCE
	{
	variableAccessSpecification	VariableAccessSpecification,
	listOfAccessResult		[0] IMPLICIT SEQUENCE OF AccessResult
	}

------------------------- GET VARIABLE ACCESS ATTRIBUTES ------------------------

GetVariableAccessAttributes-Request ::= CHOICE
	{
	name		[0] ObjectName,
	address		[1] Address
	}


GetVariableAccessAttributes-Response ::= SEQUENCE
	{
	mmsDeletable		[0] IMPLICIT BOOLEAN,
	address			[1] Address OPTIONAL,
	typeSpecification	[2] TypeSpecification
	}
--------------------------- DEFINE NAMED VARIABLE --------------------------------

DefineNamedVariable-Request ::= SEQUENCE
	{
	variableName		[0] ObjectName,
	address			[1] Address,
	typeSpecification	[2] TypeSpecification OPTIONAL
	}

DefineNamedVariable-Response ::= NULL

-------------------------- DEFINE SCATTERED ACCESS -------------------------------

DefineScatteredAccess-Request ::= SEQUENCE
	{
	scatteredAccessName		[0] ObjectName,
	scatteredAccessDescription	[1] IMPLICIT ScatteredAccessDescription
	}


DefineScatteredAccess-Response ::= NULL

------------------------- GET SCATTERED ACCESS ATTRIBUTES ------------------------

GetScatteredAccessAttributes-Request ::= ObjectName	-- ScatteredAccessName


GetScatteredAccessAttributes-Response ::= SEQUENCE
	{
	mmsDeletable			[0] IMPLICIT BOOLEAN,
	scatteredAccessDescription	[1] IMPLICIT ScatteredAccessDescription
	}

----------------------------- DELETE VARIABLE ACCESS ------------------------------

DeleteVariableAccess-Request ::= SEQUENCE
	{
	scopeOfDelete		[0] IMPLICIT INTEGER
		{
		specific		(0),
		aa-specific		(1),
		domain			(2),
		vmd			(3) 
		} DEFAULT specific,
	listOfName		[1] IMPLICIT SEQUENCE OF ObjectName OPTIONAL,
	domainName		[2] IMPLICIT Identifier OPTIONAL
	}

DeleteVariableAccess-Response ::= SEQUENCE
	{
	numberMatched	[0] IMPLICIT Unsigned32,
	numberDeleted	[1] IMPLICIT Unsigned32
	}


DeleteVariableAccess-Error ::= Unsigned32	-- numberDeleted

------------------------- DEFINE NAMED VAR. LIST -------------------------------

DefineNamedVariableList-Request ::= SEQUENCE
	{
	variableListName	ObjectName,
	listOfVariable		[0] IMPLICIT SEQUENCE OF SEQUENCE
		{
		variableSpecification 	VariableSpecification,
		alternateAccess		[5] IMPLICIT AlternateAccess OPTIONAL
		}
	}


DefineNamedVariableList-Response ::= NULL

------------------------- GET NAMED VAR. LIST ATTRIBUTES  ------------------------

GetNamedVariableListAttributes-Request ::= ObjectName	-- VariableListName


GetNamedVariableListAttributes-Response ::= SEQUENCE
	{
	mmsDeletable		[0] IMPLICIT BOOLEAN,
	listOfVariable		[1] IMPLICIT SEQUENCE OF SEQUENCE 
		{
		variableSpecification 		VariableSpecification,
		alternateAccess			[5] IMPLICIT AlternateAccess OPTIONAL
		}
	}

------------------------- DELETE NAMED VAR. LIST -------------------------------

DeleteNamedVariableList-Request ::= SEQUENCE
	{
	scopeOfDelete		[0] IMPLICIT INTEGER
		{
		specific			(0),
		aa-specific			(1),
		domain				(2),
		vmd				(3) 
		} DEFAULT specific,
	listOfVariableListName	[1] IMPLICIT SEQUENCE OF ObjectName OPTIONAL,
	domainName			[2] IMPLICIT Identifier OPTIONAL
	}


DeleteNamedVariableList-Response ::= SEQUENCE
	{
	numberMatched	[0] IMPLICIT Unsigned32,
	numberDeleted	[1] IMPLICIT Unsigned32
	}


DeleteNamedVariableList-Error ::= Unsigned32	--	number Deleted

------------------------- DEFINE NAMED TYPE -------------------------------

DefineNamedType-Request ::= SEQUENCE 
	{
	typeName		ObjectName,
	typeSpecification	TypeSpecification
	}


DefineNamedType-Response ::= NULL


------------------------- GET NAMED TYPE ATTRIB. -------------------------------

GetNamedTypeAttributes-Request ::= ObjectName -- TypeName

GetNamedTypeAttributes-Response ::= SEQUENCE
	{
	mmsDeletable		[0] IMPLICIT BOOLEAN,
	typeSpecification	TypeSpecification
	} 

------------------------- DELETE NAMED TYPE -------------------------------

DeleteNamedType-Request ::= SEQUENCE
	{
	scopeOfDelete		[0] IMPLICIT INTEGER
		{
		specific		(0),
		aa-specific		(1),
		domain			(2),
		vmd			(3) 
		} DEFAULT specific,
	listOfTypeName		[1] IMPLICIT SEQUENCE OF ObjectName OPTIONAL,
	domainName		[2] IMPLICIT Identifier OPTIONAL
	}

DeleteNamedType-Response ::= SEQUENCE
	{
	numberMatched	[0] IMPLICIT Unsigned32,
	numberDeleted	[1] IMPLICIT Unsigned32
	}

DeleteNamedType-Error ::= Unsigned32	--	number Deleted

---------------------------- SUPPORT DEFINITIONS ----------------------------

AccessResult ::= CHOICE
	{
	failure		[0] IMPLICIT DataAccessError,
	success	Data
	}


DataAccessError ::= INTEGER
	{
	object-invalidated		(0),
	hardware-fault			(1),
	temporarly-unavailable		(2),
	object-access-denied		(3),
	object-undefined		(4),
	invalid-address			(5),
	type-unsupported		(6),
	type-inconsistent		(7),
	object-attribute-inconsistent	(8),
	object-access-unsupported	(9),
	object-non-existent		(10)
	}



Data ::= CHOICE
	{
	-- context tag 0 is reserved for AccessResult
	array			[1] IMPLICIT SEQUENCE OF Data,
	structure		[2] IMPLICIT SEQUENCE OF Data,
	boolean			[3] IMPLICIT BOOLEAN,	
	bit-string		[4] IMPLICIT BIT STRING,
	integer			[5] IMPLICIT INTEGER,
	unsigned		[6] IMPLICIT INTEGER,
	floating-point		[7] IMPLICIT FloatingPoint,
	real		 	[8] IMPLICIT REAL,
	octet-string		[9] IMPLICIT OCTET STRING,
	visible-string		[10] IMPLICIT VisibleString,
	binary-time		[12] IMPLICIT TimeOfDay,
	bcd			[13] IMPLICIT INTEGER,
	booleanArray		[14] IMPLICIT BIT STRING
	}

FloatingPoint ::= OCTET STRING


VariableAccessSpecification ::= CHOICE
	{
	listOfVariable		[0] IMPLICIT SEQUENCE OF SEQUENCE
		{
		variableSpecification	VariableSpecification,
		alternateAccess		[5] IMPLICIT AlternateAccess OPTIONAL
		},
	variableListName	[1] ObjectName
	}


ScatteredAccessDescription ::= SEQUENCE OF SEQUENCE 
	{
	componentName		[0] IMPLICIT Identifier OPTIONAL,
	variableSpecification	[1] VariableSpecification,
	alternateAccess		[2] IMPLICIT AlternateAccess OPTIONAL
	}


VariableSpecification ::= CHOICE
	{
	name				[0] ObjectName,
	address				[1] Address,
	variableDescription		[2] IMPLICIT SEQUENCE
		{
		address			Address,
		typeSpecification	TypeSpecification
		},
	scatteredAccessDescription	[3] IMPLICIT ScatteredAccessDescription,
	invalidated			[4] IMPLICIT NULL
	}

Address ::= CHOICE
	{
	numericAddress		[0] IMPLICIT Unsigned32,
	symbolicAddress		[1] IMPLICIT VisibleString,
	unconstrainedAddress	[2] IMPLICIT OCTET STRING
	}


-- ********************************* SEMAPHORES *****************************************

TakeControl-Request ::= SEQUENCE
	{
	semaphoreName			[0] ObjectName,
	namedToken			[1] IMPLICIT Identifier OPTIONAL,
	priority			[2] IMPLICIT Priority DEFAULT 64,
	acceptableDelay			[3] IMPLICIT Unsigned32 OPTIONAL,
	controlTimeOut			[4] IMPLICIT Unsigned32 OPTIONAL,
	abortOnTimeOut			[5] IMPLICIT BOOLEAN OPTIONAL,
	relinquishIfConnectionLost	[6] IMPLICIT BOOLEAN DEFAULT TRUE,
	applicationToPreempt 		[7] IMPLICIT ApplicationReference OPTIONAL
	}

TakeControl-Response ::= CHOICE
	{	
	noResult		[0] IMPLICIT NULL,
	namedToken		[1] IMPLICIT Identifier
	}

-------------------------------- RELINQUISH CONTROL -----------------------------

RelinquishControl-Request ::= SEQUENCE
	{
	semaphoreName		[0] ObjectName,
	namedToken		[1] IMPLICIT Identifier OPTIONAL
	}

RelinquishControl-Response ::= NULL

------------------------------- DEFINE SEMAPHORE --------------------------------

DefineSemaphore-Request ::= SEQUENCE
	{
	semaphoreName		[0] ObjectName,
	numbersOfTokens		[1] IMPLICIT Unsigned16
	}

DefineSemaphore-Response ::= NULL

------------------------------- DELETE SEMAPHORE --------------------------------

DeleteSemaphore-Request ::= ObjectName		-- Semaphore Name

DeleteSemaphore-Response ::= NULL

--------------------------- REPORT SEMAPHORE STATUS -----------------------------

ReportSemaphoreStatus-Request ::= ObjectName	-- SemaphoreName

ReportSemaphoreStatus-Response ::= SEQUENCE
	{
	mmsDeletable		[0] IMPLICIT BOOLEAN,
	class			[1] IMPLICIT INTEGER
		{
		token 	(0),
		pool   	(1)
		},
	numberOfTokens		[2] IMPLICIT Unsigned16,
	numberOfOwnedTokens 	[3] IMPLICIT Unsigned16,
	numberOfHungTokens	[4] IMPLICIT Unsigned16
	}

--------------------------- REPORT POOL SEMAPHORE STATUS -----------------------------

ReportPoolSemaphoreStatus-Request ::= SEQUENCE
	{
	semaphoreName		[0] ObjectName,
	nameToStartAfter	[1] IMPLICIT Identifier OPTIONAL
	}

ReportPoolSemaphoreStatus-Response ::= SEQUENCE
	{
	listOfNamedTokens	[0] IMPLICIT SEQUENCE OF CHOICE
		{
		freeNamedToken		[0] IMPLICIT Identifier,
		ownedNamedToken		[1] IMPLICIT Identifier,
		hungNamedToken		[2] IMPLICIT Identifier
		},
	moreFollows		[1] IMPLICIT BOOLEAN DEFAULT TRUE
	}

--------------------------- REPORT SEMAPHORE ENTRY STATUS -----------------------------

ReportSemaphoreEntryStatus-Request ::=SEQUENCE
	{
	semaphoreName		[0] ObjectName,
	state			[1] IMPLICIT INTEGER
		{
		queued	(0),
		owner	(1),
		hung	(2)
		} ,
	entryIdToStartAfter	[2] IMPLICIT OCTET STRING OPTIONAL
	}

ReportSemaphoreEntryStatus-Response ::= SEQUENCE
	{
	listOfSemaphoreEntry 	[0] IMPLICIT SEQUENCE OF SemaphoreEntry,
	moreFollows		[1] IMPLICIT BOOLEAN DEFAULT TRUE
	}


AttachToSemaphore ::= SEQUENCE
	{
	semaphoreName			[0] ObjectName,
	namedToken			[1] IMPLICIT Identifier OPTIONAL,
	priority			[2] IMPLICIT Priority DEFAULT 64,
	acceptableDelay			[3] IMPLICIT Unsigned32 OPTIONAL,
	controlTimeOut			[4] IMPLICIT Unsigned32 OPTIONAL,
	abortOnTimeOut			[5] IMPLICIT BOOLEAN OPTIONAL,
	relinquishIfConnectionLost	[6] IMPLICIT BOOLEAN DEFAULT TRUE
	}


SemaphoreEntry ::= SEQUENCE
	{	
	entryId				[0] IMPLICIT OCTET STRING,
	entryClass			[1] IMPLICIT INTEGER
		{
		simple		(0),
		modifier 	(1)
		},
	applicationReference		[2] ApplicationReference,
	namedToken			[3] IMPLICIT Identifier OPTIONAL,
	priority			[4] IMPLICIT Priority DEFAULT 64,
	remainingTimeOut		[5] IMPLICIT Unsigned32 OPTIONAL,
	abortOnTimeOut			[6] IMPLICIT BOOLEAN OPTIONAL,
	relinquishIfConnectionLost	[7] IMPLICIT BOOLEAN DEFAULT TRUE
	}

--******************************** OPERATOR COMMUNICATION *****************************


------------------------------------------ INPUT ------------------------------------

Input-Request ::= SEQUENCE
	{
	operatorStationName	[0] IMPLICIT Identifier,
	echo			[1] IMPLICIT BOOLEAN DEFAULT TRUE,
	listOfPromptData	[2] IMPLICIT SEQUENCE OF VisibleString OPTIONAL,
	inputTimeOut		[3] IMPLICIT Unsigned32 OPTIONAL
	}


Input-Response ::= VisibleString	-- Input String

--------------------------------------- OUTPUT -------------------------------------

Output-Request ::= SEQUENCE
	{
	operatorStationName	[0] IMPLICIT Identifier,
	listOfOutputData	[1] IMPLICIT SEQUENCE OF VisibleString
	}


Output-Response ::= NULL


-- ************************************ EVENTS *********************************************

DefineEventCondition-Request ::= SEQUENCE
	{
	eventConditionName		[0] ObjectName,
	class				[1] IMPLICIT EC-Class,
	prio-rity			[2] IMPLICIT Priority DEFAULT 64,
	severity			[3] IMPLICIT Unsigned8 DEFAULT 64,
	alarmSummaryReports		[4] IMPLICIT BOOLEAN OPTIONAL,
	monitoredVariable		[6] VariableSpecification OPTIONAL,
	evaluationInterval		[7] IMPLICIT Unsigned32 OPTIONAL
	}

DefineEventCondition-Response ::= NULL


DeleteEventCondition-Request ::= CHOICE
	{
	specific		[0] IMPLICIT SEQUENCE OF ObjectName,
	aa-specific		[1] IMPLICIT NULL,
	domain			[2] IMPLICIT Identifier,
	vmd			[3] IMPLICIT NULL
	}

DeleteEventCondition-Response ::= Unsigned32	-- Candidates Not Deleted


GetEventConditionAttributes-Request ::= ObjectName	-- Event Condition Name

GetEventConditionAttributes-Response ::= SEQUENCE
	{
	mmsDeletable			[0] IMPLICIT BOOLEAN DEFAULT FALSE,
	class				[1] IMPLICIT EC-Class,
	prio-rity			[2] IMPLICIT Priority DEFAULT 64,
	severity			[3] IMPLICIT Unsigned8 DEFAULT 64,
	alarmSummaryReports		[4] IMPLICIT BOOLEAN DEFAULT FALSE,
 	monitoredVariable		[6] CHOICE
		{
		variableReference		[0] VariableSpecification,
		undefined			[1] IMPLICIT NULL
		} OPTIONAL,
	evaluationInterval		[7] IMPLICIT Unsigned32 OPTIONAL
	}


ReportEventConditionStatus-Request ::= ObjectName	-- EventConditionName

ReportEventConditionStatus-Response ::= SEQUENCE
	{
	currentState			[0] IMPLICIT EC-State,
	numberOfEventEnrollments	[1] IMPLICIT Unsigned32,
	enabled				[2] IMPLICIT BOOLEAN OPTIONAL,
	timeOfLastTransitionToActive	[3] EventTime OPTIONAL,
	timeOfLastTransitionToIdle	[4] EventTime OPTIONAL
	}


AlterEventConditionMonitoring-Request ::= SEQUENCE
	{
	eventConditionName		[0] ObjectName,
	enabled				[1] IMPLICIT BOOLEAN OPTIONAL,
	priority			[2] IMPLICIT Priority OPTIONAL,
	alarmSummaryReports		[3] IMPLICIT BOOLEAN OPTIONAL,
        evaluationInterval		[4] IMPLICIT Unsigned32 OPTIONAL
	}

AlterEventConditionMonitoring-Response ::= NULL


TriggerEvent-Request ::= SEQUENCE
	{
	eventConditionName		[0] ObjectName,
	priority			[1] IMPLICIT Priority OPTIONAL
	}

TriggerEvent-Response ::= NULL


DefineEventAction-Request ::= SEQUENCE
	{
	eventActionName              	[0] ObjectName,
	listOfModifier			[1] IMPLICIT SEQUENCE OF Modifier OPTIONAL,
	confirmed-Service-Request	[2] DefineEventAction-ConfirmedServiceRequest

	}


DefineEventAction-Response ::= NULL

DeleteEventAction-Request ::= CHOICE
	{
	specific		[0] IMPLICIT SEQUENCE OF ObjectName,
	aa-specific		[1] IMPLICIT NULL,
	domain			[3] IMPLICIT Identifier,
	vmd			[4] IMPLICIT NULL
	}

DeleteEventAction-Response ::= Unsigned32	-- candidates not deleted

GetEventActionAttributes-Request ::= ObjectName	-- Event Action Name


GetEventActionAttributes-Response ::= SEQUENCE
	{
	mmsDeletable			[0] IMPLICIT BOOLEAN DEFAULT FALSE,
	listOfModifier			[1] IMPLICIT SEQUENCE OF Modifier,
	confirmed-Service-Request	[2] DefineEventAction-ConfirmedServiceRequest
 	}

ReportEventActionStatus-Request ::= ObjectName	 -- EventActionName

ReportEventActionStatus-Response ::=  Unsigned32 -- Number of Event Enrollments


DefineEventEnrollment-Request ::= SEQUENCE
	{
	eventEnrollmentName		[0] ObjectName,
	eventConditionName		[1] ObjectName,
	eventConditionTransition	[2] IMPLICIT Transitions,
	alarmAcknowledgementRule	[3] IMPLICIT AlarmAckRule,
	eventActionName			[4] ObjectName OPTIONAL,
	clientApplication		[5] ApplicationReference OPTIONAL
	}

DefineEventEnrollment-Response ::= NULL

DefineEventEnrollment-Error ::= ObjectName


DeleteEventEnrollment-Request ::= CHOICE
	{
	specific	[0] IMPLICIT SEQUENCE OF ObjectName,
	ec		[1] ObjectName,
	ea		[2] ObjectName
	}

DeleteEventEnrollment-Response ::= Unsigned32	-- candidates not deleted


GetEventEnrollmentAttributes-Request ::= SEQUENCE
	{
	scopeOfRequest		[0] IMPLICIT INTEGER 
		{
		specific	(0),
		client		(1),
		ec		(2),
		ea		(3)
		} DEFAULT client,
	eventEnrollmentNames	[1] IMPLICIT SEQUENCE OF ObjectName OPTIONAL,
	clientApplication	[2] ApplicationReference OPTIONAL,
	eventConditionName	[3] ObjectName OPTIONAL,
	eventActionName		[4] ObjectName OPTIONAL,
	continueAfter		[5] ObjectName OPTIONAL
	}


EventEnrollment ::= SEQUENCE
	{
	eventEnrollmentName		[0] ObjectName,
	eventConditionName		[1] CHOICE
		{
		eventCondition			[0] ObjectName,
		undefined			[1] IMPLICIT NULL
		},
	eventActionName			[2] CHOICE
		{
		eventAction			[0] ObjectName,
		undefined			[1] IMPLICIT NULL
		} OPTIONAL,
	clientApplication		[3] ApplicationReference OPTIONAL,
	mmsDeletable			[4] IMPLICIT BOOLEAN DEFAULT FALSE,
	enrollmentClass			[5] IMPLICIT EE-Class,
	duration			[6] IMPLICIT EE-Duration DEFAULT current,
	invokeID			[7] IMPLICIT Unsigned32,
	remainingAcceptableDelay	[8] IMPLICIT Unsigned32 OPTIONAL
	}


GetEventEnrollmentAttributes-Response ::= SEQUENCE
	{
	listOfEventEnrollment 	[0] IMPLICIT SEQUENCE OF EventEnrollment,
	moreFollows		[1] IMPLICIT BOOLEAN DEFAULT FALSE
	}


ReportEventEnrollmentStatus-Request ::= ObjectName	-- Event Enrollment Name

ReportEventEnrollmentStatus-Response ::= SEQUENCE
	{
	eventConditionTransitions	[0] IMPLICIT Transitions,
	notificationLost		[1] IMPLICIT BOOLEAN DEFAULT FALSE,
	duration			[2] IMPLICIT EE-Duration,
	alarmAcknowledgmentRule		[3] IMPLICIT AlarmAckRule OPTIONAL,
	currentState			[4] IMPLICIT EE-State
	}

AlterEventEnrollment-Request ::= SEQUENCE
	{
	eventEnrollmentName		[0] ObjectName,
	eventConditionTransitions	[1] IMPLICIT Transitions OPTIONAL,
	alarmAcknowledgmentRule		[2] IMPLICIT AlarmAckRule OPTIONAL
	}

AlterEventEnrollment-Response ::= SEQUENCE
	{
	currentState		[0] CHOICE
		{
		state			[0] IMPLICIT EE-State,
		undefined		[1] IMPLICIT NULL
		},
	transitionTime		[1] EventTime
	}


AcknowledgeEventNotification-Request ::= SEQUENCE
	{
	eventEnrollmentName		[0] ObjectName,
	acknowledgedState		[2] IMPLICIT EC-State,
	timeOfAcknowledgedTransition	[3] EventTime
	}

AcknowledgeEventNotification-Response ::= NULL


GetAlarmSummary-Request ::= SEQUENCE
	{
	enrollmentsOnly			[0] IMPLICIT BOOLEAN DEFAULT TRUE,
	activeAlarmsOnly		[1] IMPLICIT BOOLEAN DEFAULT TRUE,
	acknowledgmentFilter		[2] IMPLICIT INTEGER 
		{
		not-acked			(0),
		acked				(1),
		all				(2) 
		} DEFAULT not-acked,
	severityFilter			[3] IMPLICIT SEQUENCE
		{
		mostSevere			[0] IMPLICIT Unsigned8,
		leastSevere			[1] IMPLICIT Unsigned8 
		} DEFAULT {mostSevere 0, leastSevere 127},
	continueAfter			[5] ObjectName OPTIONAL
	}

GetAlarmSummary-Response ::= SEQUENCE
	{
	listOfAlarmSummary		[0] IMPLICIT SEQUENCE OF AlarmSummary,
	moreFollows			[1] IMPLICIT BOOLEAN DEFAULT FALSE
	}


AlarmSummary ::= SEQUENCE
	{
	eventConditionName			[0] ObjectName,
	severity				[1] IMPLICIT Unsigned8,
	currentState				[2] IMPLICIT EC-State,
	unacknowledgedState			[3] IMPLICIT INTEGER
		{
		none		(0),
		active		(1),
		idle		(2),
		both		(3)
		},
	timeOfLastTransitionToActive		[5] EventTime OPTIONAL,
	timeOfLastTransitionToIdle		[6] EventTime OPTIONAL
	}


GetAlarmEnrollmentSummary-Request ::= SEQUENCE
	{
	enrollmentsOnly			[0] IMPLICIT BOOLEAN DEFAULT TRUE,
	activeAlarmsOnly		[1] IMPLICIT BOOLEAN DEFAULT TRUE,
	acknowledgmentFilter		[2] IMPLICIT INTEGER 
		{
		not-acked			(0),
		acked				(1),
		all				(2) 
		} DEFAULT not-acked,
	severityFilter			[3] IMPLICIT SEQUENCE
		{
		mostSevere			[0] IMPLICIT Unsigned8,
		leastSevere			[1] IMPLICIT Unsigned8 
		} DEFAULT {mostSevere 0, leastSevere 127},
	continueAfter			[5] ObjectName OPTIONAL
	}

GetAlarmEnrollmentSummary-Response ::= SEQUENCE
	{
	listOfAlarmEnrollmentSummary	[0] IMPLICIT SEQUENCE OF AlarmEnrollmentSummary,
	moreFollows			[1] IMPLICIT BOOLEAN DEFAULT FALSE
	}


AlarmEnrollmentSummary ::= SEQUENCE
	{
	eventEnrollmentName		[0] ObjectName,
	clientApplication		[2] ApplicationReference OPTIONAL,
	severity			[3] IMPLICIT Unsigned8,
	currentState			[4] IMPLICIT EC-State,
	notificationLost		[6] IMPLICIT BOOLEAN DEFAULT FALSE,
	alarmAcknowledgmentRule		[7] IMPLICIT AlarmAckRule OPTIONAL,
	enrollementState		[8] IMPLICIT EE-State OPTIONAL,
	timeOfLastTransitionToActive	[9] EventTime OPTIONAL,
	timeActiveAcknowledged		[10] EventTime OPTIONAL,
	timeOfLastTransitionToIdle	[11] EventTime OPTIONAL,
	timeIdleAcknowledged		[12] EventTime OPTIONAL
	}


EventNotification ::= SEQUENCE
	{
	eventEnrollmentName		[0] ObjectName,
	eventConditionName		[1] CHOICE
		{
		eventCondition			[0] ObjectName,
		undefined			[1] IMPLICIT NULL
		},
	severity			[2] IMPLICIT Unsigned8,
	currentState			[3] IMPLICIT EC-State OPTIONAL,
	transitionTime			[4] EventTime,
	notificationLost		[6] IMPLICIT BOOLEAN DEFAULT FALSE,
	alarmAcknowledgmentRule		[7] IMPLICIT AlarmAckRule OPTIONAL,
	actionResult			[8] IMPLICIT SEQUENCE
		{
		eventActioName			ObjectName,
		eventActionResult		CHOICE
			{
			success			[0] ConfirmedServiceResponse,
			failure			[1] IMPLICIT ServiceError
			}
		} OPTIONAL
	}


AttachToEventCondition ::= SEQUENCE
	{
	eventEnrollmentName		[0] ObjectName,
	eventConditionName		[1] ObjectName,
	causingTransitions		[2] IMPLICIT Transitions,
	acceptableDelay			[3] IMPLICIT Unsigned32 OPTIONAL
	}


EventTime ::= CHOICE
	{
	timeOfDayT			[0] IMPLICIT TimeOfDay,
	timeSequenceIdentifier		[1] IMPLICIT Unsigned32
	}


EC-Class ::= INTEGER
	{
	network-triggered	(0),
	monitored		(1)
	}

EC-State ::= INTEGER
	{
	disabled		(0),
	idle			(1),
	active			(2)
	}

EE-State ::= INTEGER
	{
	disabled		(0),
	idle			(1),
	active			(2),
	activeNoAckA		(3),
	idleNoAckI		(4),
	idleNoAckA		(5),
	idleAcked		(6),
	activeAcked		(7)
	}

Transitions ::= BIT STRING
	{
	idle-to-disabled	(0),
	active-to-disabled	(1),
	disabled-to-idle	(2),
	active-to-idle		(3),
	disabled-to-active	(4),
	idle-to-active		(5),
	any-to-deleted		(6)
	}

AlarmAckRule ::= INTEGER
	{
	none			(0),
	simple			(1),
	ack-active		(2),
	ack-all			(3)
	}

EE-Class ::= INTEGER
	{
	modifier		(0),
	notification		(1)
	}

EE-Duration ::= INTEGER
	{
	current			(0),
	permanent		(1)
	}


-- ********************************** JOURNAL *******************************************


---------------------------------- READ JOURNAL ----------------------------------

ReadJournal-Request ::= SEQUENCE
	{
	journalName			[0] ObjectName,
	rangeStartSpecification	[1] CHOICE
		{
		startingTime			[0] IMPLICIT TimeOfDay,
		startingEntry			[1] IMPLICIT OCTET STRING
		} OPTIONAL,
	rangeStopSpecification	[2] CHOICE
		{
		endingTime			[0] IMPLICIT TimeOfDay,
		numberOfEntries		[1] IMPLICIT Integer32
		} OPTIONAL,
	listOfVariables		[4] IMPLICIT SEQUENCE OF VisibleString OPTIONAL,
	entryToStartAfter	[5] IMPLICIT SEQUENCE
		{
		timeSpecification		[0] IMPLICIT TimeOfDay,
		entrySpecification		[1] IMPLICIT OCTET STRING
		}
	}

ReadJournal-Response ::= SEQUENCE
	{
	listOfJournalEntry		[0] IMPLICIT SEQUENCE OF JournalEntry,
	moreFollows			[1] IMPLICIT BOOLEAN DEFAULT FALSE
	}


JournalEntry ::= SEQUENCE
	{
	entryIdentifier		[0] IMPLICIT OCTET STRING,
	originatingApplication		[1] ApplicationReference,
	entryContent			[2] IMPLICIT EntryContent
	}

---------------------------------- WRITE JOURNAL ----------------------------------

WriteJournal-Request ::= SEQUENCE
	{
	journalName			[0] ObjectName,
	listOfJournalEntry		[1] IMPLICIT SEQUENCE OF EntryContent
	}

WriteJournal-Response ::= NULL

-------------------------------- INITIALIZE JOURNAL ----------------------------------

InitializeJournal-Request ::= SEQUENCE
	{
	journalName			[0] ObjectName,
	limitSpecification		[1] IMPLICIT SEQUENCE
		{
		limitingTime			[0] IMPLICIT TimeOfDay,
		limitingEntry			[1] IMPLICIT OCTET STRING OPTIONAL
		} OPTIONAL
	}

InitializeJournal-Response ::= Unsigned32	-- entries deleted

---------------------------------- REPORT JOURNAL STATUS -----------------------------

ReportJournalStatus-Request ::= ObjectName	-- Journal Name

ReportJournalStatus-Response ::= SEQUENCE
	{
	currentEntries		[0] IMPLICIT Unsigned32,
	mmsDeletable		[1] IMPLICIT  BOOLEAN
	}	

---------------------------------- CREATE JOURNAL ----------------------------------

CreateJournal-Request ::= SEQUENCE
	{
	journalName	[0] ObjectName
	}

CreateJournal-Response ::= NULL

---------------------------------- DELETE JOURNAL ----------------------------------

DeleteJournal-Request ::= SEQUENCE
	{
	journalName	[0] ObjectName
	}

DeleteJournal-Response ::= NULL


-------------------------------- SUPPORTING PRODUCTIONS ----------------------------

EntryContent ::= SEQUENCE
	{
	occurenceTime		[0] IMPLICIT TimeOfDay,
	additionalDetail	[1] JOU-Additional-Detail OPTIONAL,
		-- additionalDetail shall be omitted
		-- from abstract syntax defined in this standard
	entryForm		 CHOICE
		{
		data			[2] IMPLICIT SEQUENCE
			{
			event			[0] IMPLICIT SEQUENCE
				{
				eventConditionName	[0] ObjectName,
				currentState		[1] IMPLICIT EC-State
				} OPTIONAL,
			listOfVariables	[1] IMPLICIT SEQUENCE OF SEQUENCE
				{
				variableTag		[0] IMPLICIT VisibleString,
				valueSpecification	[1] Data
				} OPTIONAL
			},
		annotation		[3] IMPLICIT VisibleString
		}
	}


JOU-Additional-Detail ::= NULL	-- Defined by Companion Standard



-- **************************************** FILES *********************************************

ObtainFile-Request ::= SEQUENCE {
	sourceFileServer	[0] IMPLICIT ApplicationReference OPTIONAL,
	sourceFile		[1] IMPLICIT FileName,
	destinationFile		[2] IMPLICIT FileName
	}

ObtainFile-Response ::= NULL

ObtainFile-Error ::= INTEGER {
	source-file	 (0),
	destination-file (1)
	}


FileOpen-Request ::= SEQUENCE {
	fileName	[0] IMPLICIT FileName,
	initialPosition	[1] IMPLICIT Unsigned32
	}

FileOpen-Response ::= SEQUENCE {
	frsmID		[0] IMPLICIT Integer32,
	fileAttributes	[1] IMPLICIT FileAttributes
	}

FileRead-Request ::= Integer32

FileRead-Response ::= SEQUENCE {
	fileData	[0] IMPLICIT OCTET STRING,
	moreFollows	[1] IMPLICIT BOOLEAN DEFAULT TRUE
	}

FileClose-Request ::= Integer32

FileClose-Response ::= NULL


FileRename-Request ::= SEQUENCE {
	currentFileName	[0] IMPLICIT FileName,
	newFileName	[1] IMPLICIT FileName
	}

FileRename-Response ::= NULL

FileRename-Error ::= INTEGER {
	source-file	 (0),
	destination-file (1)
	}

FileDelete-Request ::= FileName

FileDelete-Response ::= NULL


FileDirectory-Request ::= SEQUENCE {
	fileSpecification	[0] IMPLICIT FileName OPTIONAL,
	continueAfter		[1] IMPLICIT FileName OPTIONAL
	}

FileDirectory-Response ::= SEQUENCE {
	listOfDirectoryEntry	[0] SEQUENCE OF DirectoryEntry,
	moreFollows		[1] IMPLICIT BOOLEAN DEFAULT FALSE
	}

DirectoryEntry ::= SEQUENCE {
	filename		[0] IMPLICIT FileName,
	fileAttributes		[1] IMPLICIT FileAttributes
	}


FileAttributes ::= SEQUENCE {
	sizeOfFile	[0] IMPLICIT Unsigned32,
	lastModified	[1] IMPLICIT GeneralizedTime OPTIONAL
	}
