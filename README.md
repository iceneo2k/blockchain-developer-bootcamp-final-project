# blockchain-developer-bootcamp-final-project

Title:
Decentralized certificate of education, training or competency

Overview:
Online courses and assessments are a valuable tool and can provide individuals with a stepping stone to a new career or new chapter in their lives.
When a respected organization or body issues a certificate of completion to an individual, that certificate may be used as a basis for a  job offer.

How can the company offering the job verify the authenticity of the certificate?

In this case, a certificate issued on the Ethereum blockchain could be used.

The principle:

- An organization issuing the certificate would have their ENS address TXT record within their DNS. 

- The individual would sign in to the online course of the organization with their Eth identity, e.g. “Sign in with Ethereum” button.

- The course would create a ‘course completion’ contract which is automatically validated when some condition is met – e.g. final exam pass > 80%. (not sure how this would be done yet, maybe just the cert is generated at the end of the course for now).

- The contract would contain metadata containing the course title and the body issuing the certificate’s DNS to verify the ENS/Eth address against their TXT records.

- An independent front-end UI would allow any other organization to view the course certificates associated with an Eth address in a user-friendly manner.

- When an interested third party (e.g. a potential new employer) wishes to verify that the person they are talking to is indeed the holder of these certificates they would use the UI to send a link to the certificate holder containing a pub key encrypted string. 

- The certificate holder would reply with the decrypted string confirming that they are indeed the holder of that certificate.
