# cwa-remediation-packages
Copyright © 2019 Symantec Corporation. All rights reserved.

Symantec, the Symantec Logo, the Checkmark Logo and  are trademarks or registered trademarks of Symantec Corporation or its affiliates in the U.S. and other countries. Other names may be trademarks of their respective owners.

This Symantec product may contain third party software for which Symantec is required to provide attribution to the third party (ìThird Party Programsî). Some of the Third Party Programs are available under open source or free software licenses. The License Agreement accompanying the Software does not alter any rights or obligations you may have under those open source or free software licenses. Please see the Third Party Legal Notice Appendix to this Documentation or TPIP ReadMe File accompanying this Symantec product for more information on the Third Party Programs.

The product described in this document is distributed under licenses restricting its use, copying, distribution, and decompilation/reverse engineering. No part of this document may be reproduced in any form by any means without prior written authorization of Symantec Corporation and its licensors, if any.

THE DOCUMENTATION IS PROVIDED "AS IS" AND ALL EXPRESS OR IMPLIED CONDITIONS, REPRESENTATIONS AND WARRANTIES, INCLUDING ANY IMPLIED WARRANTY OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE OR NON-INFRINGEMENT, ARE DISCLAIMED, EXCEPT TO THE EXTENT THAT SUCH DISCLAIMERS ARE HELD TO BE LEGALLY INVALID. SYMANTEC CORPORATION SHALL NOT BE LIABLE FOR INCIDENTAL OR CONSEQUENTIAL DAMAGES IN CONNECTION WITH THE FURNISHING, PERFORMANCE, OR USE OF THIS DOCUMENTATION. THE INFORMATION CONTAINED IN THIS DOCUMENTATION IS SUBJECT TO CHANGE WITHOUT NOTICE.

The Licensed Software and Documentation are deemed to be commercial computer software as defined in FAR 12.212 and subject to restricted rights as defined in FAR Section 52.227-19 "Commercial Computer Software - Restricted Rights" and DFARS 227.7202, et seq. "Commercial Computer Software and Commercial Computer Software Documentation," as applicable, and any successor regulations, whether delivered by Symantec as on premises or hosted services. Any use, modification, reproduction release, performance, display or disclosure of the Licensed Software and Documentation by the U.S. Government shall be solely in accordance with the terms of this Agreement.

Symantec Corporation
350 Ellis Street
Mountain View, CA 94043
https://www.symantec.com
---------------------------------------------------------------------------------------------------------------------
The remediation feature of Cloud Workload Assurance provides details of failed checks in the remediation input payload to fix the misconfigurations that are observed on AWS resources. You can either use the lambda scripts provided by CWA, or use an alternate method to fix the failed checks. After the issues are fixed, remediation output payload is generated  and an update can be sent to CWA. You can scan your resources to verify the fixes. You can monitor the remediation process by referring to the CloudWatch logs of lambda. 

You can configure remediation using the CFT provided by CWA or complete the steps manually. 

For detailed information about the remediation feature, refer to the following link:
https://help.symantec.com/cs/SCWP/SCWA/v131001445_v127279924/About-remediation-in-Cloud-Workload-Assurance?locale=EN_US


The cwa-remediation-packages folder contains the following files:


* SYMC_CWA_Remdiation_CFT.json
  Symantec Cloud Workload Assurance CFT for remediation. 

* SYMC_CWA_Remediation_Orchestrator.zip
  Symantec Cloud Workload Assurance remediation orchestrator lambda.


* SYMC_CWA_CLR_API_call.zip
  Symantec Cloud Workload Assurance remediation Public API to update remediation status in CWA 
	

* SYMC_CWA_Remediation_Worker_CloudTrail.zip
  Symantec Cloud Workload Assurance Remediation worker lambda to fix certain CloudTrail checks.

* SYMC_CWA_Remediation_Worker_IAMPassword.zip
  Symantec Cloud Workload Assurance Remediation worker lambda to fix certain IAMPassword checks.

* SYMC_CWA_Remediation_Worker_KMS.zip
  Symantec Cloud Workload Assurance Remediation worker lambda to fix certain KMS checks.

* SYMC_CWA_Remediation_Worker_S3.zip
  Symantec Cloud Workload Assurance Remediation worker lambda to fix certain S3 checks.


