THE FOLLOWING NOTES APPLY ONCE THE YOCTO LINUX IMAGE IS BUILT AND ROOTFS IS POPULATED:
======================================================================================
Use "murata-master" sub-folder for module-specific CLM_BLOB file (CLM_BLOB filename includes Murata module designation). 
Note that the FMAC driver loads a specific NVRAM filename when coming up: "cyfmac"+<CYW number>+<-sdio or -pcie>+".clm_blob"
This means that for any Murata modules which share the same chipset, we can only have one CLM_BLOB file present in the default folder: "/lib/firmware/cypress".
For example, 2EA and 2EC share the same CLM_Blob file.

The following module CLM_BLOB default files are included in this folder: 

The following table lists out the "md5sum" for all the CLM_BLOB files.
-----------------------------------------------------------------------------------------------
|   File Name                                 |		md5sum                   | Murata     |
|                                             |                                  | Regulatory |
|				              |                                  | Certified  |	
|---------------------------------------------|----------------------------------|------------|
| cyfmac43012-sdio.1LV.clm_blob               | 0fb69b76a77dc8d9af62eab1bca2ef69 |     Yes    |
| cyfmac43022-sdio.2GF.STA.clm_blob           | 90cd50c20dd0844cee2f9062bafacc05 |     Yes    |
| cyfmac43022-sdio.2GF.OutdoorSTA.clm_blob    | 955fc84c538801ce2bdc24e0b68efbeb |     Yes    |
| cyfmac43022-sdio.2GF.IndoorAP.clm_blob      | 2ebc1eb7cbebc63abcd3f981a375676e |     Yes    |
| cyfmac43022-sdio.2GF.OutdoorAP.clm_blob     | fa8f29a58698d8a9e8f40c441c259601 |     Yes    |
| cyfmac43455-sdio.1MW.clm_blob               | dfb5979f56bc869302417a0df9798188 |     Yes    |
| cyfmac43430-sdio.1DX.clm_blob               | 966becd509a2fc8f30f27fa0dab4673e |     Yes    |
| cyfmac43430-sdio.1FX.clm_blob               | 966becd509a2fc8f30f27fa0dab4673e |     Yes    |
| cyfmac43430-sdio.1LN.clm_blob               | 966becd509a2fc8f30f27fa0dab4673e |     No     |
| cyfmac43455-sdio.1HK.clm_blob               | 4aafba3e50ac9756aebcb89b81979023 |     No     |
| cyfmac43455-sdio.1LC.clm_blob               | 4aafba3e50ac9756aebcb89b81979023 |     No     |
| cyfmac4354-sdio.1BB.clm_blob                | 39404def8b34d793bd8aebf86fd9ede7 |     No     |
| cyfmac4359-sdio.1WZ.clm_blob                | 9fc5b48fd08e593e0339b2c0450e1337 |     No     |
| cyfmac4373-sdio.2AE.clm_blob                | 2ee452fab031bcf712af0c75929e428c |     Yes    |
| cyfmac4373-sdio.2BC.clm_blob                | 2ee452fab031bcf712af0c75929e428c |     Yes    |
| cyfmac43439-sdio.1YN.clm_blob	              | 47fa101aac57c643a612754b6a05537a |     Yes    |
| cyfmac4356-pcie.1CX.clm_blob                | f8611ec4459ebadf99bb999e5903df12 |     No     |
| cyfmac54591-pcie.1XA.clm_blob	              | 0eff4b59e0ffc5f1babc865bd05897c0 |     Yes    |
| cyfmac54591-sdio.2BZ.clm_blob	              | 0eff4b59e0ffc5f1babc865bd05897c0 |     Yes    |
| cyfmac55572-sdio.2EA.clm_blob	              | 0e51f9477d3f1a43f0406424ddc0b9c5 |     No     |
| cyfmac55572-pcie.2EA.clm_blob	              | 22a59428cac2011e466c04fa08170ee9 |     No     |
| cyfmac55572-pcie.2EA.clm_blob_APIndoor      | d3bf7bebd74745339c336dd4b81e8ef5 |     Yes    |
| cyfmac55572-pcie.2EA.clm_blob_APOutdoor     | 7b9e3e7b38788b689dbe3d836b47ed89 |     Yes    |
| cyfmac55572-pcie.2EA.clm_blob_STAIndoor     | 29fb4b4f5c210cb5cafc49753445bf45 |     Yes    |
| cyfmac55572-pcie.2EA.clm_blob_STAOutdoor    | d9e29c11ee83459933b6f753c88fa132 |     Yes    |
| cyfmac55572-sdio.2EA.clm_blob_APIndoor      | d3bf7bebd74745339c336dd4b81e8ef5 |     Yes    |
| cyfmac55572-sdio.2EA.clm_blob_APOutdoor     | 7b9e3e7b38788b689dbe3d836b47ed89 |     Yes    |
| cyfmac55572-sdio.2EA.clm_blob_STAIndoor     | 29fb4b4f5c210cb5cafc49753445bf45 |     Yes    |
| cyfmac55572-sdio.2EA.clm_blob_STAOutdoor    | d9e29c11ee83459933b6f753c88fa132 |     Yes    |
-----------------------------------------------------------------------------------------------
