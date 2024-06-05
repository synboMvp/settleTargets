## 入驻项目信息提交
Please submit the project using a feature branch, add a new folder in the "projects" folder, and use the project name as the naming convention, example: **synboProtocol**, and make sure the folder name is unique.     

You can then add project basic information files, project details files, AMA files, and terms files to this folder.     

**1、 Project basic information file**     
*Naming convention*: Use camel case naming, name it after the project name, and end with .json.       
     Example: **synboProtocol.json**      
*File content*: Contains the document fields below, please read carefully.       

**2. Project details file**     
***Naming convention***: The file name starts with info_, plus the project name, and ends with .md.     
     Example: **info_synboProtocol.md**    
***File content***: A detailed project overview, project details information provided through visual and text documents. Contents may include but are not limited to:     
1、Project overview: Detailed description of the background, goals, and features of the project.     
2、Team details: Introduce team members and their backgrounds.   
3、Token economy: Describe the issuance mechanism, allocation plan, and purpose of the token.    
4、Roadmap: The future development plan and timeline of the project.   
5、Historical fundraising information: including information such as financing rounds, amounts, and investors.    

**3. AMA file**   
***Naming convention***: The file name starts with ama_, plus the project name, and ends with .md.   
     Example: **ama_synboProtocol.md**   
***File content***: Interact with users in the form of questions and answers   

**4. Terms file**   
***Naming convention***: The file name starts with terms_, plus the project name, and ends with .md.   
     Example: **terms_synboProtocol.md**  
***File content***: Describe the project's terms of use and policies in detail, including but not limited to:   
1、Terms of Service: Services provided by the project and their conditions of use.   
2、Privacy Policy: How user data is collected, used, and protected.   
3、Disclaimer: The project party's statement of responsibility for users' use of project services.   

After submission, it will be reviewed by a dedicated team member and merged into the main branch. Project information will only be visible on the merged website.    

**The following is the fields included in the project basic information file, please read carefully:** 

"IDs by automatically generated": {    
"Data-ID":"Automatically generated, only one for a project.",    
"IPFS-ID[Data-ID]":"Automatically generated, only one for a project on IPFS",    
"Target-IDs[IPFS-ID][chain-ids]":"Automatically generated, one ID for one chain",    
"Contractor[Target-ID][n]":"Automatically generated, one chain can have multiple Contractors"    
},   

"project": {    
"name": "Required, project name, such as SYNBO protocol",    
"description one sentence": "Required, this is a sentence of 50 characters or less to introduce a project",    
"logo": "Required, project logo image, 120*120, base64, svg, less than 1M",    
"bannerImage": "Optional, banner image, 1440*400, base64, svg, less than 1M",    
"chains": "Required, the ecosystem it is in, such as: "ETH, BNB", etc.,    
"tags": "Required, such as: DEFI, DAO, LAYER2..., industry standard identifiers for easy classification and browsing"    
},    

"token[]": [    
{
"name":"Optional, token name, such as SYNBO",    
"symbol":"Optional, token symbol, such as SYT",    
"where-chain":"Optional, which chain is the token on? ”,    
“contractAddress”:“Optional, if it is erc20, then display contractAddress”,    
“totalSupply”:“Optional, format: 100,000.000”,    
“valuation”:“Optional, the valuation of the last round of financing, format: 100,000.000”,    
“circulatingSupply”:“Optional, format: 100,000.000”,    
“tokenType”:“Optional, ERC-20 or Native_TOKEN”,    
“description”:“Optional, a description of the role, utility or life cycle of the current token in the project. "    
},    
{    
"...":""     
}    
],    
“project-social”: {    
“website”: "",    
“twitter”: "",    
“telegram”: "",   
“github”: "",    
“medium”: "",    
“discord”: "",    
“email”: ""    
}

