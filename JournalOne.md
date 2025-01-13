## Journal Submission One 

|  | Details |
| :---------: | :-------------: |
| Date Range  | 14 Oct - 1 Nov 2024  |
| Mentor  | Alexander Scheel  |
| Mentee  | Fatima Patel |

###  ${\color{Teal} \textnormal{14 - 15 Oct}}$
🖋️ **Emails Discussing Mentorship Details and Project Ideas**  
* Covered time commitment and availability, project goals, and the structure for progress reporting.

📖 **RFC 5280: Internet X.509 Public Key Infrastructure Certificate and CRL Profile**  
* Browsed through the docs to understand X.509 Version 3 Certificate and Certificate extensions better.
 
📖 **Went over these Vault tutorials**  
* [Tokens](https://docs.hashicorp.com/vault/tutorials/get-started/introduction-tokens), [Policies](https://docs.hashicorp.com/vault/tutorials/get-started/introduction-policies) and [Roles](https://docs.hashicorp.com/vault/tutorials/get-started/introduction-roles)
  
💻 **[Issue #459](https://github.com/openbao/openbao/issues/459) PKI - Allow revocation of expired certificates**    
* Looked into use cases and started modifying code.   
* Recreated the issue on my environment. 

💻 **[Vault #27609](https://github.com/hashicorp/vault/issues/27609) [Vault #19452](https://github.com/hashicorp/vault/issues/19452)**   
* Looked into issues & comments connected to [Issue #459](https://github.com/openbao/openbao/issues/459).

💻 **[Bao API/PKI Documentation](https://openbao.org/api-docs/secret/pki/#tidy)**    
* Went through parameter definitions and tested them out on dev server to aid with solving [Issue #459](https://github.com/openbao/openbao/issues/459)

💡 **API-First Approach**   
* Make API responses consistent and predictable so clients don’t have to do redundant checks, hence reducing complexity.

###  ${\color{Teal} \textnormal{16 - 17 Oct}}$

💻 **Create Draft of First Blog Post**   

💻 **Created [draft PR](https://github.com/openbao/openbao/pull/638) for Issue #459**   
* Added allow_expired_cert_revocation field and checked there's no issues parsing.     
* Update revocation behavior.       
* Create tests for revoking expired-but-not-revoked certificates.   

###  ${\color{Teal} \textnormal{18 Oct}}$
🖋️ **First Mentorship Meeting**   
* Confirmed my understanding of the Issue #459   
* Discussed issue #27219 of vault, agreed we should delete the invalid certificates   
* Discussed how revoked_safety_buffer should work alongside safety_buffer   
💻 **Still working on [PR](https://github.com/openbao/openbao/pull/638) for Issue #459**    


###  ${\color{Teal} \textnormal{21 - 23 Oct}}$
💻 **Created [draft PR](https://github.com/openbao/openbao/pull/653) as a follow up for my prev [PR](https://github.com/openbao/openbao/pull/638)**      
* Ensured revoked_safety_buffer defaults to safety_buffer when unset.     
   Had a bit of a hard time figuring this one out because of the pointers.      
* Created test to check if revoked_safety_buffer and safety_buffer values are correctly set and defaulted.     
  
###  ${\color{Teal} \textnormal{24 - 25 Oct}}$         
💻 **Completed implementation for [revoked_safety_buffer](https://github.com/openbao/openbao/pull/653).**     
* Created corresponding tests and updated current tests.       
 
###  ${\color{Teal} \textnormal{28 Oct}}$      
💻 **Pulled issue [Tidy and revoke error out on certificates with duplicate extension](https://github.com/openbao/openbao/issues/659) from Vault.**      
