## Journal Submission Two 

|  | Details |
| :---------: | :-------------: |
| Date Range  | 1 Nov - 26 Nov |
| Mentor  | Alexander Scheel  |
| Mentee  | Fatima Patel |

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

###  ${\color{Teal} \textnormal{25 - 26 Nov}}$
* Go over path_tidy.go and backend_test.go and add comments.
* Create plugin autors guide.
* Revise RFC parameters.
* Resolve comments on tidy pagination.
