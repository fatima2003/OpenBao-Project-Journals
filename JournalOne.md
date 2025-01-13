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


###  ${\color{Teal} \textnormal{1 Nov}}$
🖋️ **Mentorship Meeting**


###  ${\color{Teal} \textnormal{8 Nov}}$
* Managed to get more detailed response info in `path_fetch.go`
  
🖋️ **Mentorship Meeting**    
* Discussed ways to test pagination in tidy and how metrics work.      
* Confirmed `-detailed` response can be under another path so that it can be ACL'ed 
and to save on resources since response includes all details even if the flag is not specified.   
* Other PKI enhancements: Vault #26037 (Imported Issuer Clarity), Vault #27248    
  
###  ${\color{Teal} \textnormal{11 - 14 Nov}}$
* Clean up docs for delete invalid certs & return extra details PR's.    
* Read RFC by Gabriel, Policy Unions, transactional storage.    
* Add flag for user to define page size.    
* Rebase + Add test to tidy pagination.    

###  ${\color{Teal} \textnormal{15 Nov}}$
🖋️ **Mentorship Meeting**
* Discussed Policy Unions:
    * People mentioned adding policies was restricting access instead of adding if a policy with less priveledges was added.
    * Policies with priorities (mentioned by Janma): If policies overlap, higher priority wins.
    * Concluded CEL could be a good idea to try and solve this problem.


###  ${\color{Teal} \textnormal{22 Nov}}$
🖋️ **Mentorship Meeting**
* Go over RFC- CEL for ceritificate issuance.
* Discuss details of where to put plugin authors guide.
* Discussed auto removal of ACL Policies.
* Discussed where to house CEL files for RFC.
* Got insight on how PR reviews are done.

###  ${\color{Teal} \textnormal{25 -16 Nov}}$
* Go over path_tidy.go and backend_test.go and add comments.
* Create plugin autors guide.
* Revise RFC parameters.
* Resolve comments on tidy pagination.

###  ${\color{Teal} \textnormal{27 Nov}}$
* remove depreciated `.Subjects()`
🖋️ **Mentorship Meeting**
* What should be the structure for plugin authors guide.
* Bao is default deny.

###  ${\color{Teal} \textnormal{1 Dec}}$
* Read over ACME and OCSP.
* create Named Issuer Clarity Issue.
* create handleListPage() Issue.
* Read over docs for PKI secrets enegine considerations.

###  ${\color{Teal} \textnormal{12 Dec}}$
🖋️ **Mentorship Meeting**
* Working on updating certs and cert chains to have TTL 100 years.
* Discussed how to go about Imported Issuer Clarity.

###  ${\color{Teal} \textnormal{17 Dec}}$
* Created 100 yr TTL cert chains.
* Browse through Kubernetes CEL code.
* Create CEL paths.
* Complete create CEL role API.

###  ${\color{Teal} \textnormal{20 Dec}}$
🖋️ **Mentorship Meeting**
* Discussed nits of RFC:
    * Should failure policy be case insensitive and have abbreviated versions?
    * Where should CEL injectable functions be housed?

###  ${\color{Teal} \textnormal{6 Jan}}$
* Add `key_type` and `key_bits` to cel/issue.


###  ${\color{Teal} \textnormal{10 Jan}}$
🖋️ **Mentorship Meeting**
* Went over RFC progress, should we keep the parameter `failure_policy`?
