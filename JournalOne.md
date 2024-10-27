## Journal Submission One 

|  | Details |
| :---------: | :-------------: |
| Date Range  | 14 Oct - 1 Nov 2024  |
| Mentor  | Alexander Scheel  |
| Mentee  | Fatima Patel |

####  ${\color{Teal} \textnormal{14 - 15 Oct}}$
> 
> 🖋️ **Emails Discussing Mentorship Details and Project Ideas**  
> $\quad$ $\space$ Covered time commitment and availability, project goals, and the structure for progress reporting.
>
> 📖 **RFC 5280: Internet X.509 Public Key Infrastructure Certificate and CRL Profile**  
> $\quad$ $\space$ Browsed through the docs to understand X.509 Version 3 Certificate and Certificate extensions better.
> 
> 📖 **Went over these Vault tutorials**  
> $\quad$ $\space$ [Tokens](https://docs.hashicorp.com/vault/tutorials/get-started/introduction-tokens), [Policies](https://docs.hashicorp.com/vault/tutorials/get-started/introduction-policies) and [Roles](https://docs.hashicorp.com/vault/tutorials/get-started/introduction-roles)
> 
> 💻 **[Issue #459](https://github.com/openbao/openbao/issues/459) PKI - Allow revocation of expired certificates**    
> $\quad$ $\space$ Looked into use cases and started modifying code.   
> $\quad$ $\space$ Recreated the issue on my environment. 
>
> 💻 **[Vault #27609](https://github.com/hashicorp/vault/issues/27609) [Vault #19452](https://github.com/hashicorp/vault/issues/19452)**   
> $\quad$ $\space$ Looked into issues & comments connected to [Issue #459](https://github.com/openbao/openbao/issues/459).
> 
> 💻 **[Bao API/PKI Documentation](https://openbao.org/api-docs/secret/pki/#tidy)**    
> $\quad$ $\space$ Went through parameter definitions and tested them out on dev server to aid with solving [Issue #459](https://github.com/openbao/openbao/issues/459)
>
> 💡 **API-First Approach**   
> $\quad$ $\space$ Make API responses consistent and predictable so clients don’t have to do redundant checks, hence reducing complexity.
> 
####  ${\color{Teal} \textnormal{16 - 17 Oct}}$
>
> 💻 **Create Draft of First Blog Post**   
> $\quad$ $\space$ 
>
> 💻 **Created [draft PR](https://github.com/openbao/openbao/pull/638) for Issue #459**   
> $\quad$ $\space$ Added allow_expired_cert_revocation field and checked there's no issues parsing.     
> $\quad$ $\space$ Update revocation behavior.       
> $\quad$ $\space$ Create tests for revoking expired-but-not-revoked certificates.   
>
> 🖋️ **TSC Meeting**   
> $\quad$ $\space$


####  ${\color{Teal} \textnormal{18 Oct}}$
> 🖋️ **First Mentorship Meeting**   
> $\quad$ $\space$ Confirmed my understanding of the Issue #459   
> $\quad$ $\space$ Discussed issue #27219 of vault, agreed we should delete the invalid certificates   
> $\quad$ $\space$ Discussed how revoked_safety_buffer should work alongside safety_buffer   
> 💻 **Still working on [PR](https://github.com/openbao/openbao/pull/638) for Issue #459**    


####  ${\color{Teal} \textnormal{21 - 23 Oct}}$
> 💻 **Created [draft PR](https://github.com/openbao/openbao/pull/653) as a follow up for my prev [PR](https://github.com/openbao/openbao/pull/638)**      
> $\quad$ $\space$ Ensured revoked_safety_buffer defaults to safety_buffer when unset.     
> $\quad$ $\space$ $\quad$ $\space$ Had a bit of a hard time figuring this one out because of the pointers.      
> $\quad$ $\space$ Created test to check if revoked_safety_buffer and safety_buffer values are correctly set and defaulted.     
  
####  ${\color{Teal} \textnormal{24 - 25 Oct}}$         
> 💻 **Completed implementation for [revoked_safety_buffer](https://github.com/openbao/openbao/pull/653).**     
> $\quad$ $\space$ Created corresponding tests and updated current tests.       
 
####  ${\color{Teal} \textnormal{28 Oct}}$      
> 💻 **Pulled issue [Tidy and revoke error out on certificates with duplicate extension](https://github.com/openbao/openbao/issues/659) from Vault.**      
> $\quad$ $\space$ 

####  ${\color{Teal} \textnormal{1 Nov}}$
> 🖋️ **Second Mentorship Meeting**   
> $\quad$ $\space$
> 



